pipeline {
    agent any
    stages {
        stage("Deploy") {
            input {
                message "Ready to deploy?"
                ok "Yes"
                submitter "ssbostan,admin,admins,managers"
                submitterParameter "SUBMITTER_USERNAME"
            }
            steps {
                echo "Deployment stage."
            }
        }
    }
}