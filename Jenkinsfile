pipeline {
    agent {
        label 'git-websites'
    }

    stages {
        stage('trigger-netbeans-site-build') {

            steps {
                triggerRemoteJob remotePathMissing: [$class: 'StopAsFailure'], remotePathUrl: 'jenkins://712657a46c181b3ff60d2c029abcf8b7/Netbeans/netbeans-antora-organization/netbeans-antora/main'            
            }
        }
    }
}
