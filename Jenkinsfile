def DOCKER_IMAGE_BRANCH = ""
def GIT_REPOSITORY_URL = "https://github.com/akhazov/identidock.git"

pipeline {
    agent {
        docker {
            image 'alpine'
        }
    }
    parameters {
        booleanParam(name: 'COMPILE', defaultValue: true, description: 'Compile this value')
        booleanParam(name: 'DEPLOY', defaultValue: false, description: 'Deploy this value')
    }
    stages {
        stage("Init repo") {
            steps {
                sh 'hostname'
                sh 'ls'
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
        stage("Deploy") {
            steps {
            when {
                '${param.DEPLOY}' true
            }
                echo "Этап 3"
            }
        }
    }
}