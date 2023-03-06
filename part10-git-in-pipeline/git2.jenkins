pipeline {
    agent any
    stages {
        stage("Clone Git Repository") {
            steps {
                dir("neptune") {
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
}