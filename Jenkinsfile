pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
                echo params.Branch
                sh 'dd if=/dev/urandom of=more.bin bs=1M count=10'
                archiveArtifacts artifacts: 'more.bin', followSymlinks: false
                sh 'sleep 15'
                echo 'Done!'
            }
        }
    }
}
