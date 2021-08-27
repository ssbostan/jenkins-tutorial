pipeline {
    agent any
    environment {
        SAMPLE_GLOBAL_ENV_VAR = "Test global ENV variables."
    }
    stages {
        stage("Build") {
            environment {
                SAMPLE_STAGE_ENV_VAR = "Test stage ENV variables."
            }
            steps {
                echo "Build stage."
                echo "$SAMPLE_GLOBAL_ENV_VAR"
                echo "$SAMPLE_STAGE_ENV_VAR"
            }
        }
        stage("Test") {
            steps {
                echo "Test stage."
                echo "$env.SAMPLE_GLOBAL_ENV_VAR"
            }
        }
        stage("Release") {
            steps {
                echo "Release stage."
                echo "${SAMPLE_GLOBAL_ENV_VAR}"
            }
        }
    }
}