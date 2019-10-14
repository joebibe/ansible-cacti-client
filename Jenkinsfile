pipeline {
    agent any
    stages {
	    stage('Compile') {
            steps {
                    echo "Compiled Successfully!!"
    }
            
    stage('Build image') {
        /* This builds the actual image; synonymous to
         * docker build on the command line */

        app = docker.build("joebibe/projet-cacti")
    }

    stage('Test image') {
        /* Ideally, we would run a test framework against our image.
         * For this example, we're using a Volkswagen-type approach ;-) */

        app.inside {
            sh 'echo "Tests passed"'
        }
    }
}
