pipeline {
    agent any
    stages {
        stage("Notify") {
            // when { triggeredBy "SCMTrigger" }
            // when { triggeredBy "TimerTrigger" }
            // when { triggeredBy "UpstreamCause" }
            when { triggeredBy(cause: "UserIdCause", detail: "ssbostan") }
            steps {
                echo "Notify whom may concern."
            }
        }
    }
}