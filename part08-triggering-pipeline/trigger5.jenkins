pipeline {
    agent any
    triggers {
        upstream(
            upstreamProjects: "myproject",
            threshold: hudson.model.Result.UNSTABLE
        )
    }
    stages {
        stage("Test") {
            steps {
                echo "Hello World!"
            }
        }
    }
}