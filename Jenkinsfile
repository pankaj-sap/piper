@Library('piper-lib-os') _
node() {
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    sudo chmod 666 /var/run/docker.sock
    
        stage('build') {
    mtaBuild script: this
}
}
