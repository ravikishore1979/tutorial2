@Library('piper-lib-os') _
node() {
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    stage('CopyConfig') {
	echo "Test scrip"
    }
    stage('build') {
    mtaBuild script: this
    }
    stage('deploy') {
    cloudFoundryDeploy script: this
   }
}
