pipeline {
    agent any
    stages {
        stage('Example') {
            steps { 
                echo 'Hello World'
                script{
                    dir(nihao){
                        git credentialsId:"9e69170b-00d6-4878-a3e3-b456cc30529a",url:"https://github.com/xiaoxiaozengzen/jenkins.git" 
                    }
                }
            }
        }
    }
}
