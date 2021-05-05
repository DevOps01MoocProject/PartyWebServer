pipeline {
    agent {label EC2CloudAgent}
    
    
    stages {      
        stage('Run Server') {
            steps {
                script {
                    sh "docker build -t ducluanxutrieu/node_party_web_server ."
                    sh "docker run -p 49160:3005 -d ducluanxutrieu/node_party_web_server"
                }
            }
        }
    }
}
