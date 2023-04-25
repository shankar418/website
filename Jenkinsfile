pipeline
{
  
  agent {label 'node2'}
  
  stages
  {
    stage('Build')
    {
      steps
      {
        sh "sudo docker build -t masterapp ."
      }
    }
       
  }  
  
}

