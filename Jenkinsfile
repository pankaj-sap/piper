@Library('piper-lib-os') _
node() {
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
dir('/Users/pankaj'){    
        stage('build') {
    mtaBuild script: this
        }
}
}
