pipeline {
    agent any
    triggers {
        GenericTrigger(
            causeString: "Triggered from Webhook",
            token: "unique-token-to-start-the-current-pipeline"
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