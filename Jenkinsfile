pipeline {
    agent {
    node {
        label 'AGENT-1'
        
    }
}
    // build
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    // after build execution post is used check the status of execution 
    post { 
        always { 
            echo 'I will always say Hello again!'
        }
        failure { 
            echo 'The jenkins script is failed'
        }
        success { 
            echo 'The jenkins script is passed successfully'
        }
        
    }
    
    }
}


