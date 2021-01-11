node {
        stage('Git clone') {
        git credentialsId: 'github_root', url: 'https://github.com/paavani25/ks.git'
        }
		stage('clean') {
		sh 'mvn clean'
		}
		stage('compile') {
		sh 'mvn compile'
		}
		stage('package') {
		sh 'mvn package'
		}
		stage('deploy') {
		sh 'mvn deploy'
		}
}
