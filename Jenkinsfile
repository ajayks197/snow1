pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building.1.'
                pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building1..'
				import hudson.model.*

def payloadString = build.buildVariableResolver.resolve("payload")

payloadObject = new groovy.json.JsonSlurper().parseText(payloadString)

targetCommit = payloadObject.pull_request.head.sha

build.addAction(new ParametersAction(new StringParameterValue('targetCommit', targetCommit)))
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}

            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
