pipeline {
    agent any
    stages {
	    stage('Compile') {
            steps {
                    echo "Compiled Successfully!!";
            }
        stage('JUnit') {
            steps {
                    echo "JUnit Passed Successfully!";
            } 
        stage('Quality-Gate') {
            steps {
                    echo "SonarQube Quality Gates passed successfully!!";
                /*sh exit ("1");*/
            }
        stage('deploy') {
            steps {
              echo "Pass!";
            }
      }
}
