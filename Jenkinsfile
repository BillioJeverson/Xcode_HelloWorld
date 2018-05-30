pipeline {
    agent { label 'iOS' }
    stages {
        stage('Build') {
        	steps {
        		sh 'xcodebuild -project HelloWorld.xcodeproj -scheme "HelloWorld" -destination \'platform=iOS Simulator,name=iPhone 6\''
        	}	
        }
    }
}