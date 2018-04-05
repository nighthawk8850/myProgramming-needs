def workspace
node 
{
    
    stage('Checkout')
    {
        
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '4b201dac-7210-4bf2-b0ea-a6ab85d06c86', url: 'https://github.com/samsonawane/SampleProject.git']]])
        workspace = pwd()
        
    }
    stage('Statistical Code Analysis')
        {
            echo 'Statistic Code Analysis'
        }
        
    stage('Build Code')
    
        {
            echo 'Build code'
        }
        
    stage('Unit Test')
        {
            echo 'Unit Test'
        }
        
    stage('Delivery')
        {
            echo 'Deliver the Code'
        }
    
}
