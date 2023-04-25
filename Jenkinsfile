pipeline
{
  
  agent {label 'node1'}
  
  stages
  {
    stage('Build')
    {
      steps
      {
        sh "sudo docker build -t masterapp ."
        sh "sudo docker rm -f $(sudo docker ps -a -q)
      }
    }
       
  }  
  
}

