pipeline {
    agent any
    environment {
        ENV = "testing"
    }
    stages {
        stage("Test") {
            when {
                environment(name: "ENV", value: "testing")
            }
            steps {
                echo "Test stage."
            }
        }
    }
}