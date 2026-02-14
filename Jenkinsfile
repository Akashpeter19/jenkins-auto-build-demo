pipeline {
    agent any
    stages {
        stage('Run Script') {
            steps {
                sh './hello.sh'
            }
        }
    }
    post {
        success {
            mail to: 'impeter2245@gmail.com',
                 subject: "Jenkins Build Success",
                 body: "Build completed successfully for hello.sh"
        }
        failure {
            mail to: 'impeter2245@gmail.com',
                 subject: "Jenkins Build Failed",
                 body: "Build failed. Check Jenkins console."
        }
    }
}
