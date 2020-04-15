
pipeline
{
  agent any
  
  tools
  {
    nodejs 'node'
  }
  stages
  {
    stage('Build')
    {
      steps
      {
        script
        {
          checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '${RepoBranch}']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'GitHub_credential', url: 'https://github.com/pankajy1/react-web-app.git']]]
        }
      }
    }
  }
}
