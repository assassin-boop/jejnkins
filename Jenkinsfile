pipeline{
    agent any
    stages{
        stage('checkout'){
            steps{
                deleteDir()
                sh '''
                    git clone https://github.com/assassin-boop/jejnkins.git
                    ls -l
                '''
                }
        }
        stage('deploy'){
            steps{
                sh '''
                    rm -rf /var/www/html/*
                    cp -r jejnkins/* /var/www/html
                '''
            }
            
        }
    }
}
