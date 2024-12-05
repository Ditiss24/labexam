pipeline {
    agent any  

    stages {
        stage('Checkout') {
            steps {
               
		sh 'https://github.com/Ditiss24/labexam.git '               
                
            }
        }

        stage('Run Shell Script') {
            steps {
                script {
                    
                    sh 'chmod +x show_datetime.sh'

                   
                    sh './show_datetime.sh'
                }
            }
        }
    }

    post {
        always {
            
            echo "Pipeline finished"
        }
    }
}

