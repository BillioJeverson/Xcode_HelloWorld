pipeline {
    agent {
    	docker{
    		image 'mattpaletta/xcbuild:latest'
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