pipeline { 
    agent any 
    stages {
        stage('Clone repository') { 
            steps { 
                git url: 'https://github.com/Apachy999/Jenkins'
            }
        }
        stage('Checking repository'){
            steps { 
        new_branch
                sh "ls -la"

        master
            }
        }
        stage('Packing project') {
            steps {
                sh '''
                tar -zcvf /tmp/package.tar.gz  ./
                '''
                deleteDir()
                sh "mv /tmp/package.tar.gz  ./"
            }
        }
        stage('Packing test') {
            steps {
                sh "ls -la"
            }
        }
    }
}
