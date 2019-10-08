pipeline {
    agent none
    stages {
        stage('Ubuntu 16.04') {
    	    agent { docker { image 'ubuntu:16.04' } }
            steps {
                sh 'cat /etc/*release*'
            }
        }
       stage('Ubuntu 18.04') {
    	    agent { docker { image 'ubuntu:18.04' } }
            steps {
                sh 'cat /etc/*release*'
            }
        }
        stage('Second stage'){
	    agent any
            steps {
		sh 'sleep(10)'
	    }
        }
    }
}
