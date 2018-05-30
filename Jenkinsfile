pipeline {
    agent { label 'iOS' }
    stages {
    	stage('Checkout'){
    		steps{
    			$class: 'GitSCM',
            	branches: [[name: 'master']],
            	doGenerateSubmoduleConfigurations: false,
            	extensions: [], submoduleCfg: [],
            	userRemoteConfigs: [[
                	name: 'github',
                	url: 'https://github.com/BillioJeverson/Xcode_HelloWorld'
                ]]
    		}
    	}
        stage('Build') {
        	steps {
        		sh 'xcodebuild -workspace Xcode_HelloWorld/HelloWorld.xcodeproj/project.xcworkspace/ -scheme "HelloWorld" -destination \'platform=iOS Simulator,name=iPhone 6\''
        	}
        }
    }
}