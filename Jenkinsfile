
pipeline{ 
  agent any
    stages{
      stage("1st"){
        steps{
          echo 'I am SMART'
          sh 'ls -l'
          sh 'kubectl get pods --kubeconfig /admin.conf'
          echo 'yeahhhhhhhhh'
        }
      }
    }  
}
