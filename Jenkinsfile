pipeline
{
  
  agent {label 'node1'}
  
  stages
  {
    stage('Build')
    {
      steps
      {
        //sh "sudo docker rm -f ${sudo docker ps -a -q}"
        sh "sudo docker build -t masterapp ."
      }
    }
    stage('Website')
    {
    steps
      {
        sh "sudo docker run -itd --rm -p 82:80 --name website-container masterapp"
      }
    }
  }  
  
}
