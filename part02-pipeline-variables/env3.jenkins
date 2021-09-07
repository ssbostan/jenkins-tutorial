pipeline {
    agent any
    environment {
        MYUSERPASS = credentials("test-user-pass")
    }
    stages {
        stage("Test") {
            steps {
                // Do not use " for command methods like sh, bat, powershell, pwsh, etc.
                // Use ' to avoid groovy interpolation and command injection vulnerabilities.
                sh 'echo $MYUSERPASS'
                sh 'logintest --username $MYUSERPASS_USR --password $MYUSERPASS_PSW'
            }
        }
    }
}
