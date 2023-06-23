pipeline {
    agent any
    stages {
        stage("Test") {
            when {
                beforeAgent true
                beforeInput true
                beforeOptions true
                // Write your conditions here. For example:
                equals(actual: currentBuild.number, expected: 1)
            }
            steps {
                echo "Hello World!"
            }
        }
    }
}
