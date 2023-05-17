pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
               
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
