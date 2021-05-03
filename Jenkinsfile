
pipeline{ 
  agent any
    stages{
      stage("1st"){
        steps{
          echo 'I am SMART'
          sh 'ls -l'
          sh 'kubectl apply -f deploy.yml --kubeconfig=/admin.conf'
        }
      }
    }  
}
