node {
    stage('SCM Checkout') {
        git credentialsId: 'github-cred', url: 'https://github.com/joebibe/ansible-cacti-client.git'
    }
    stage('Mvn Package'){
        def mvnHome = tool name: 'maven-3', type: 'maven'
        def mvnCMD = "${mvnHome}/bin/mvn"
        sh "${mvnCMD} clean package"
    }
}
        

