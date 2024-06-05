
pipeline {
    agent any

    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'master', url: 'https://github.com/NUCESFAST/scd-final-lab-exam-haniyatj'
            }
        }

        stage('Build Frontend') {
            steps {
                dir('./client') {
                    script {
                        sh 'npm install'
                    }
                }
            }
        }
        
        stage('Build and Deploy Backend 1') {
            steps {
                dir('./Classrooms') {
                    script {
                        // Assuming you use npm for Node.js backend
                        sh 'npm install'
                        // Other build and deployment commands for backend 1
                    }
                }
            }
        }

        stage('Build and Deploy Backend 2') {
            steps {
                dir('./event-bus') {
                    script {
                        sh 'npm install'
                    }
                }
            }
        }

        stage('Build and Deploy Backend 3') {
            steps {
                dir('./Post') {
                    script {
                        sh 'npm install'
                    }
                }
            }
        }
    }
}
