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
      }
    }
    stage('Website')
    {
    steps
      {
        sh "sudo docker run -itd -p 82:80 --name website-container masterapp"
      }
    }
    
  }  
  
}
