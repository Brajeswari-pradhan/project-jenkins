// pipeline {
//     agent any

//     stages {
//         stage('Checkout') {
//             steps {
//                 echo 'Checkout stage'
//             }
//         }

//         stage('Build') {
//             steps {
//                 echo 'Build stage'
//             }
//         }

//         stage('Test') {
//             steps {
//                 echo 'Test stage'
//             }
//         }

//         stage('Docker Build') {
//             steps {
//                 echo 'Docker build stage'
//             }
//         }
//     }
// }
//-------------------------------------------------------------------------new-------------------------------------------------------------------------
@Library('my-shared-lib') _

pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Build stage'
            }
        }

        stage('Test') {
            steps {
                runTests()
            }
        }

        stage('Docker Build') {
            steps {
                dockerBuild("myapp:latest")
            }
        }
    }
}
