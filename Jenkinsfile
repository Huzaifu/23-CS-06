pipeline{
    agent any

    stages{
        stage('checkout'){
            steps{
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '3e232842-522e-441d-bb39-a4b5014e8039', url: 'https://github.com/Huzaifu/Huzaifa_Sarfraz_23-CSE-06.git']])
            }

        }

        stage(Run the index file on the webserver){
            steps{
               sh cp index.html /var/www/html/
            }
        }
    }
}
