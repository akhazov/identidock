def DOCKER_IMAGE_BRANCH = ""
def GIT_REPOSITORY_URL = "https://github.com/akhazov/identidock.git"

pipeline {
    sh 'hostname'
    agent {
        docker {
            image 'alpine'
        }
    }
    stages {
        stage("Init repo") {
            steps {
                git url: "${GIT_REPOSITORY_URL}",
                    branch: 'master'
            }
        }
        stage("Compile") {
            steps {
                sh 'hostname'
                sh 'ls'
            }
        }
        stage("Build Docker Image") {
            steps {
                echo "Этап 3"
            }
        }
    }
}