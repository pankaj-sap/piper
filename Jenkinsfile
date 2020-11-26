@Library('piper-lib-os') _
node() {
    stage('prepare') {
                    echo 'Pankaj'
            
        echo env.BUILD_USER_ID

        checkout scm
        setupCommonPipelineEnvironment script:this
    }
   
        stage('build') {
            echo env.BUILD_USER_ID
    mtaBuild script: this
        }

}
