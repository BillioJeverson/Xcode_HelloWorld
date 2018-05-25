pipeline {
    agent {
    	docker{
    		image 'brikis98/docker-osx-dev'
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