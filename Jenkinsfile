pipeline {
    agent any
    stages {
        stage('Clonar repositório') {
            steps {
                git(
                    branch: 'main', 
                    url: 'https://github.com/raphaelpcarlos/TESTE-MOBILE-EBAC-SHOP.git'
                )
            }
        }

        stage('Instalar dependências') {
            steps {
                sh 'npm install'
            }
        }

        stage('Rodar Testes') {
            steps {
                sh 'npm test'
            }
        }
    }
}
