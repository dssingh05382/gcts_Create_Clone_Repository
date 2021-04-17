@Library('piper-lib-os') _
node() {
    stage('prepare') { 
		gctsCreateRepository(
		  script: this,
		  host: 'https://fc-pun01-hana.india.rapidigm.com:8001',
		  client: '300',
		  abapCredentialsId: 'ABAPUserPasswordCredentialsId',
		  repository: 'DEV003',
		  remoteRepositoryURL: 'https://github.com/skondekar/shubh',
		  role: 'SOURCE',
		  vSID: 'S4A'
		  )	
	}
}
node() {
    stage('prepare') { 
		gctsCloneRepository(
		  script: this,
		  host: 'https://fc-pun01-hana.india.rapidigm.com:8001',
		  client: '300',
		  abapCredentialsId: 'ABAPUserPasswordCredentialsId',
		  repository: 'DEV003'
		)	
	}
}
