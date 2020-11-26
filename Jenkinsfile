@Library('piper-lib-os') _
def job = Jenkins.getInstance().getItemByFullName(env.JOB_BASE_NAME, Job.class)
def build = job.getBuildByNumber(env.BUILD_ID as int)
def userId = build.getCause(Cause.UserIdCause).getUserId()
node() {
    stage('prepare') {
                    echo 'Pankaj'
        
            
        echo userId

        checkout scm
        setupCommonPipelineEnvironment script:this
    }
   
        stage('build') {
            echo env.BUILD_USER_ID
    mtaBuild script: this
        }

}
