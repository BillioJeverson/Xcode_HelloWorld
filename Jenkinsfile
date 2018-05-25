pipeline {
    agent {
    	docker{
    		image 'nginx'
    	}
    }
    stages {
        stage('Build') {
        	steps {
        		sh 'xcodebuild -scheme "HelloWorld" -configuration "Debug"
        	}
        }
    }
}