pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                changeset "**/*.py"
            }
            steps {
                echo "Hello World!"
            }
        }
    }
}