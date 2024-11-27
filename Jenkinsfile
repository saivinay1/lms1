pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'cd webapp && sudo docker container run --rm -e SONAR_HOST_URL="http://3.20.204.179:9000" -e SONAR_LOGIN=" sqp_a36e97f382fe1eb878d61ba81b35de8d81c2f5f4" -v ".:/usr/src" sonarsource/sonar-scanner-cli -Dsonar.projectKey=lms'
            }
        }
    }
}