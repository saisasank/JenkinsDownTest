node("master"){
	stage('Clean Workspace'){
		cleanWs()
	}
	
	stage('Code Checkout'){
		checkout([$class: 'GitSCM', branches: [[name: "master"]], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: "https://github.com/saisasank/JenkinsDownTest"]]])
	}
	
	stage('CommitID'){
		sh "ls -la"
		sh "echo ${COMMIT}"
	}
}
