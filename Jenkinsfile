pipeline {
    agent {
        label 'ec2'
    }

    stages {
        stage('Deploy the container') {
            steps {
                
                sh 'docker pull hellosircodeplay/gfg27img'
                sh 'docker rm -f webos1'
                sh 'docker run -dit --name webos1 -p 81:80 hellosircodeplay/gfg27img'
            }
        }
    }
}
