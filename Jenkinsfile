def DOCKER_IMAGE_BRANCH = ""
def GIT_REPOSITORY_URL = "https://github.com/akhazov/identidock.git"

pipeline {
    agent {
        docker {
            image 'alpine'
        }
    }
    stages {
        stage("Init repo") {
            steps {
                git url:{$GIT_REPOSITORY_URL},
                    branch: 'master'
            }
        }
    }
}