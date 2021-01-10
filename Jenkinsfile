def DOCKER_IMAGE_BRANCH = ""
def GIT_REPOSITORY_URL = "https://github.com/akhazov/identidock.git"

pipeline {
    agent any
    stages {
        stage("Init repo") {
            steps {
                git url:{$GIT_REPOSITORY_URL},
                    branch: 'master'
            }
        }
        stage("Compile") {
            steps {
                sh 'git --version'
            }
        }
        stage("Build Docker Image") {
            steps {
                sh 'echo "Этап 3"'
            }
        }
    }
}