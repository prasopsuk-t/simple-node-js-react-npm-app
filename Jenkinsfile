pipeline {
    agent any
    stages {
        stage ('build') {
            steps {
                bat 'npm install'
            }
        }
        stage ('Run Powershell Command') {
            steps {
                echo 'Start Executing'
                script {
                    powershell '''
                        Write-Output "Hello world"
                        $date = Get-Date
                        Write-Output "Current Date and time : $date"
                    '''
                }
            }
        }

    }
}