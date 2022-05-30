pipeline {
    agent any
    stages {
        stage("Test") {
            steps {
                catchError(
                    message: "Error inside the catchError block"
                ) {
                    sh "false"
                }
                mail(
                    subject: "Error in Pipeline",
                    body: "An error occurred in the Jenkins pipeline.",
                    from: "jenkins@localhost",
                    to: "ssbostan@linuxmail.org"
                )
            }
        }
    }
}