pipeline {
    agent any
    triggers {
        cron "* * * * *"
    }
    stages {
        stage("Test") {
            steps {
                echo "Hello World!"
            }
        }
    }
}