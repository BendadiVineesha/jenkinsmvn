def workspace;
node{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '995dfb6a-38fe-4190-b056-1e17bf2709d3', url: 'https://github.com/BendadiVineesha/jenkinsmvn.git']]])
    workspace=pwd()
        
    }
    stage('Static Code Analysis')
    {
      echo "static code analysis"  
    }
    stage('Build')
    {
        echo "build the code"
    }
    stage('Delivary')
    {
        echo "delivar the code"
    }
    stage('Email Notification'){
        mail bcc: '', body: 'welcome to gmail alerts', cc: '', from: '', replyTo: '', subject: 'jenkins', to: 'vineeshabendadi2@gmail.com'
    }
}
