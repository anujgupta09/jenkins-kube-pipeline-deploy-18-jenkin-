
pipeline{ 
  agent any
    stages{
      stage("1st"){
        when{
          false
        }
        steps{
          echo 'I am SMART'
          sh 'ls -l'
          sh "kubectl apply -f deploy.yml --kubeconfig admin.conf"
          sh "kubectl get pods --kubeconfig admin.conf"
          echo 'yeahhhhhhhhh'
        }
      }
    }  
}
