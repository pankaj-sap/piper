@Library('piper-lib-os') _
node() {
    stage('prepare') {
                    echo 'Pankaj'
        def job = Jenkins.getInstance().getItemByFullName(env.JOB_BASE_NAME, Job.class)
def build = job.getBuildByNumber(env.BUILD_ID as int)
def userId = build.getCause(Cause.UserIdCause).getUserId()
            
        echo userId

        checkout scm
        setupCommonPipelineEnvironment script:this
    }
   
        stage('build') {
            echo env.BUILD_USER_ID
    mtaBuild script: this
        }

}
