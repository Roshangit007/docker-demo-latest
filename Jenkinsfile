pipeline{
    agent any

    stages{

        stage('login server'){

            steps{
            sshagent(credentials:['jenkins-server']){

                sh 'ssh  -o StrictHostKeyChecking=no  root@172.31.13.73 uptime "whoami"'

            }

                echo "success lgoin"

            }
        }
    }
}