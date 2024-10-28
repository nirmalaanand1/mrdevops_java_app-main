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
    }
}