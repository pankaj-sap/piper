library('piper-lib-os')
node(){
        bat "set"
    withMaven {
        git changelog: false, poll: false, url: 'https://github.com/jtnord/maven-test-project.git'
        
        bat "mvn package"
    }

stage('build') {
    mtaBuild script: this
}
}
