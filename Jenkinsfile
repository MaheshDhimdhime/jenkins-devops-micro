// //SCRIPTED
// node {
// 		echo "Build"
// 		echo "Test"
// 		echo "Test"
// }

pipeline {
    agent {docker {image 'maven:3.6.3'}}

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
    post{
        always{
            echo 'i am awesome .I run always'
        }
        success{
            echo 'I am When you are successful'
        }
        failure{
            echo 'I run when you fail'
        }
    }
}