pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                equals(actual: currentBuild.number, expected: 1)
            }
            steps {
                echo "Hello World!"
            }
        }
    }
}