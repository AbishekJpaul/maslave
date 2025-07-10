pipeline {
    agent any

    stages {
        stage('Doctor') {
            steps {
                echo 'Provides medical care and helps people stay healthy or recover from illness'
            }
        }
        stage('Engineer') {
            steps {
                echo 'Designs and builds machines, structures, or systems (civil, software, mechanical, etc.)'
            }
        }
        stage('Teacher') {
            steps {
                echo 'Educates students and helps shape future generations'
            }
        }
        stage('Lawyer') {
            steps {
                echo 'Represents clients in legal matters and ensures justice is served'
            }
        }
        stage('Software Developer') {
            steps {
                echo 'Writes code to create apps, websites, and digital systems'
            }
        }
        stage('Architect') {
            steps {
                echo 'Plans and designs buildings and structures'
            }
        }
        stage('Police Officer') {
            steps {
                echo 'Protects public safety and enforces the law'
            }
        }
        stage('Chef') {
            steps {
                echo 'Prepares meals and often creates recipes in restaurants or hotels'
            }
        }
        stage('Journalist') {
            steps {
                echo 'Investigates and reports news to inform the public'
            }
        }
        stage('Farmer') {
            steps {
                echo 'Grows crops and raises animals to provide food and raw materials'
            }
        }
    }

    post {
        success {
            emailext (
                to: 'anyoneelsekill@gmail.com',
                subject: "SUCCESS: ${env.JOB_NAME} [${env.BUILD_NUMBER}]",
                body: "Good news! Job ${env.JOB_NAME} #${env.BUILD_NUMBER} succeeded.\nCheck it here: ${env.BUILD_URL}"
            )
        }
        failure {
            emailext (
                to: 'anyoneelsekill@gmail.com',
                subject: "FAILURE: ${env.JOB_NAME} [${env.BUILD_NUMBER}]",
                body: "Uh-oh! Job ${env.JOB_NAME} #${env.BUILD_NUMBER} failed.\nSee details: ${env.BUILD_URL}"
            )
        }
    }
}
