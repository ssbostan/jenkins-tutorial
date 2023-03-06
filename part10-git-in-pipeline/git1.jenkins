pipeline {
    agent any
    stages {
        stage("Clone Git Repository") {
            steps {
                git(
                    url: "https://github.com/ssbostan/neptune.git",
                    branch: "master",
                    changelog: true,
                    poll: true
                )
            }
        }
    }
}