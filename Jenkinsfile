node (){
	 def mvnHome = tool 'Maven3'
		stage('Build')
		{
		 checkout([$class: 'GitSCM', 
		 branches: [[name: '*/master']],
		 doGenerateSubmoduleConfigurations: false,
		 extensions: [], 
		 submoduleCfg: [], userRemoteConfigs: [[credentialsId: '9f904bac-0d2d-4e74-bb3f-b9a0f7a364de', url: 'https://github.com/bsreenua6/CounterWebapp.git']]])
		 
		 bat '%{mvnHome}%/bin/mvn clean install'
		}
	}


