pipeline {
    agent {
    	docker{
    		image 'pragneshpatel/xcode'
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