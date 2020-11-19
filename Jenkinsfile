library('piper-lib-os')
node(){
        sh "set"
    withMaven {
        git changelog: false, poll: false, url: 'https://github.com/jtnord/maven-test-project.git'
        
        sh "mvn package"
    }

stage('build') {
    mtaBuild script: this
}
}
