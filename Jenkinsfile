@Library('piper-lib-os') _
node() {
    stage('Create Repository') { 
		gctsCreateRepository(
		  script: this,
		  host: 'http://10.34.156.145:8002',
		  client: '300',
		  abapCredentialsId: 'ABAPUserPasswordCredentialsId',
		  repository: 'DEV003',
		  remoteRepositoryURL: 'https://github.com/skondekar/shubh',
		  role: 'SOURCE',
		  vSID: 'S4D'
		  )	
	}
}
node() {
    stage('Clone Repository') { 
		gctsCloneRepository(
		  script: this,
		  host: 'http://10.34.156.145:8002',
		  client: '300',
		  abapCredentialsId: 'ABAPUserPasswordCredentialsId',
		  repository: 'DEV003'
		)	
	}
}
