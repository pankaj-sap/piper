@Library('piper-lib-os') _
node() {
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
dir('../users/pankaj'){    
        stage('build') {
    mtaBuild script: this
        }
}
}
