@Library('shared-lib') _

pipeline {
    agent any

    stages {

        stage('Initialize') {
            steps {
                echo "Pipeline Started..."
                buildInfo()
            }
        }

        stage('Build') {
            steps {
                echo "Simulating Build Process..."
                sh 'echo Building project...'
            }
        }

        stage('Test') {
            steps {
                echo "Simulating Test Stage..."
                sh 'echo Running tests...'
            }
        }
    }

    post {

        success {
            emailext(
                subject: "SUCCESS: ${env.JOB_NAME} #${env.BUILD_NUMBER}",
                body: """
Build Successful

Job: ${env.JOB_NAME}
Build: ${env.BUILD_NUMBER}
URL: ${env.BUILD_URL}
""",
                to: "akashpeterp@gmail.com"
            )
        }

        failure {
            emailext(
                subject: "FAILED: ${env.JOB_NAME} #${env.BUILD_NUMBER}",
                body: """
Build Failed

Job: ${env.JOB_NAME}
Build: ${env.BUILD_NUMBER}
URL: ${env.BUILD_URL}
""",
                to: "akashpeterp@gmail.com"
            )
        }
    }
}

