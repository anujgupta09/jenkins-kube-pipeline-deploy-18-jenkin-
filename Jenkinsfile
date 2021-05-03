
pipeline{
  agent any
  parameters{
  booleanParam(name: "isdeploy" , defaultValue: false)
  }
    stages{
      stage("1st"){
        when{
          expression {
              params.isdeploy
          }
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
