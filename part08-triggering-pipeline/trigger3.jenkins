pipeline {
    agent any
    triggers {
        pollSCM "*/10 * * * *"
    }
    stages {
        stage("Test") {
            steps {
                echo "Hello World!"
            }
        }
    }
}