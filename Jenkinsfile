pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/your-repo-url.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Deploy to EC2') {
            steps {
                sh '''
                ssh -o StrictHostKeyChecking=no ec2-user@your-ec2-public-ip << 'EOF'
                cd /var/www/html
                git pull origin main
                sudo systemctl restart nginx
                EOF
                '''
            }
        }
    }
}
Add Jenkinsfile for automated deployment
