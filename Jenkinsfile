pipeline {
    agent {
    	docker{
    		image 'jkingyens/docker4xcode'
    	}
    }
    stages {
        stage('Build') {
        	steps {
        		sh 'xcodebuild -scheme "HelloWorld" -configuration "Debug"'
        	}
        }
    }
}