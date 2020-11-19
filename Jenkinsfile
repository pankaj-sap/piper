@Library('piper-lib-os') _
node() {
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
dir('./pankaj'){    
        stage('build') {
    mtaBuild script: this
        }
}
}
