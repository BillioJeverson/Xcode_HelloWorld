pipeline {
    agent { label 'iOS' }
    stages {
        stage('Build') {
        	steps {
        		sh 'xcodebuild -workspace /Users/billiojeverson/Desktop/HelloWorld.xcodeproj/project.xcworkspace/ -scheme "HelloWorld" -destination \'platform=iOS Simulator,name=iPhone 6\''
        	}
        }
    }
}