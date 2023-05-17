pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "sudo -S npm  install"
                sh "sudo -S npm  run build"
            }
        }
        stage("Deploy") {
            steps {
                sh "sudo rm -rf /var/www/cicd"
                sh "sudo cp -r ${WORKSPACE}/build/ /var/www/cicd/"
            }
        }
    }
}
