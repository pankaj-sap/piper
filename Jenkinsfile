@Library('piper-lib-os') _

node() {
    stage('prepare') {
                    echo 'Pankaj'
        User.current().getId()
        
        def specificCause = currentBuild.getBuildCauses('hudson.model.Cause$UserIdCause')
if (specificCause) {
    println("Executed by user $specificCause.userName")
    //echo "specificCause: $specificCause"
    //echo "specificCause: ${specificCause.userId[0]}"
    echo "specificCause: $specificCause.userName"
    echo "specificCause: ${specificCause.userName}"
    //echo "specificCause: $specificCause.shortDescription"
}
        
            
        

        checkout scm
        setupCommonPipelineEnvironment script:this
    }
   
        stage('build') {
            echo env.BUILD_USER_ID
    mtaBuild script: this
        }

}
