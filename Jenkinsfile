node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/sweathagulabi/pom.git']]])
    
    }
    stage('build')
    {
        echo "build"
    }

}
