pipeline {
    agent any
    triggers {
        upstream "my-upstream-project1"
        // upstream "my-upstream-project1,my-upstream-project2"
    }
    stages {
        stage("Test") {
            steps {
                echo "Hello World!"
            }
        }
    }
}