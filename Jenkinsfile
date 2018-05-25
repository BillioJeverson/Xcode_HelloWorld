pipeline {
    agent {
    	docker{
    		image 'zhaoseagull/xcode'
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