pipeline {
    agent any

    stages {
        stage('检出') {
            steps {
                echo 'Building..'
            }
            parallel {
                         stage('parallel 检出1') {
                            
                                steps {
                                     echo "parallel 检出1"
                                      }
                             }
                            stage('parallel 检出2') {
                            
                                steps {
                                    echo "parallel 检出1"
                                     }               
                        }
                    }
        stage('测试') {
            steps {
                echo 'Testing..'
            }
        }
        stage('部署') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
