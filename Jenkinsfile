pipeline{
    agent any

    stages{
       stage ('Git'){
         steps{
              git branch :'master',
              url : ' https://github.com/ouss01/DevOps-Pipe-1.git',
              git credentialsId: 'git_credentials'

              }
        }

       }


        }
    }