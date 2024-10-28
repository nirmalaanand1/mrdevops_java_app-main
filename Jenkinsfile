@Library('jenkins_shared_lib') _

pipeline{
    agent any

    stages{
        stage('Git Checkout'){
            steps{
                script{
                    gitCheckout(
                    branch: 'main',
                    url: 'https://github.com/nirmalaanand1/mrdevops_java_app-main.git'
                  )
                }
            }
        }
        stage('Unit Test maven'){
            steps{
                script{
                    mvnTest()
                }
            }
        }
        stage('Integration Test maven'){
            steps{
                script{
                    mvnIntegrationTest()
                }
            }
        }
    }
}