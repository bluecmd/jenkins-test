pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World - development edition'
                echo params.Branch
                sh 'sleep 15'
                echo 'Done!'
            }
        }
    }
}
