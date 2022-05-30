pipeline {
    agent any
    stages {
        stage("Test") {
            steps {
                echo isUnix() ? "Unix-like agent." : "Windows agent."
            }
        }
    }
}