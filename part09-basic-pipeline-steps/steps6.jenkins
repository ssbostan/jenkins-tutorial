pipeline {
    agent any
    stages {
        stage("Test") {
            steps {
                retry(10) {
                    sleep(5)
                    timeout(time: 3, unit: "SECONDS") {
                        sh "python mysqlcheck.py"
                    }
                }
            }
        }
    }
}