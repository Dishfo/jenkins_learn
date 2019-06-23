pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('build') {
            environment {
              TAG = 'Dishfo'
            }
            steps {
                sh 'mvn --version'
                sh '''
                  echo "hello world"
                  ls -lah
                  echo $TAG
                '''
            }
        }
    }

    post {
      always {
        echo "always"
      }
    }
}
