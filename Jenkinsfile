pipeline {
 agent any
 stages {
 stage('Check Git') {
    steps {
        sh 'git --version'
    }
}
 stage('Clone') {
    steps {
        git branch: 'main',
            url: 'https://github.com/AdityaRaj1010/SeleniumMaven.git'
    }
}
 stage('Build') {
	 steps {
	 	sh 'mvn clean compile'
	 }
 }
 stage('Test Automation') {
	 steps {
	 	sh 'mvn test'
	 }
 }
 }
}
