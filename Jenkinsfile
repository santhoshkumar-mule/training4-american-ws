pipeline {
    agent any
    stages { 
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
}

def triggerCause = currentBuild.rawBuild.getCause(org.jenkinsci.plugins.pipeline.github.trigger.IssueCommentCause)

if (triggerCause) {
    echo("Build was started by ${triggerCause.userLogin}, who wrote: " +
         "\"${triggerCause.comment}\", which matches the " +
         "\"${triggerCause.triggerPattern}\" trigger pattern.")
} else {
    echo('Build was not started by a trigger')
}