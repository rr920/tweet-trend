pipeline {
    agent {
        node {
            label 'maven'
        }
    }

    stages {
        stage("Build") {
            steps {
                echo "--------------------Build Started---------------------"
                sh 'mvn clean deploy -Dmaven.test.skip=true'
                echo "-------------------Build Completed--------------------"
            }
        }
    }
}

