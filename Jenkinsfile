pipeline {
    agent any

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
                echo 'Hansible...🤣'
                ansiblePlaybook becomeUser: 'ubuntu', credentialsId: 'ansible', inventory: 'host.ini', playbook: 'flask-deploy.yml'
            }
        }
    }
}
