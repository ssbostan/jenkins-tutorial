pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                changelog ".*Test.*"
            }
            steps {
                echo "Hello World!"
            }
        }
    }
}