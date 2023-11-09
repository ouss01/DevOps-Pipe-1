pipeline{
    agent any

    stages{
       stage ('Git'){
         steps{
              git branch :'master',
              url : ' https://github.com/ouss01/DevOps-Pipe-1.git',
              credentialsId: 'git_credentials'

              }
        }
       stage ('MVN Clean')
              {
               steps{
                      sh 'mvn clean -DskipTests'
                 }
              }
               stage ('MVN compile')
              {
               steps{
                      sh 'mvn compile'
                    }
                }
                 stage ('build package')
                {
                 steps{
                        sh 'mvn package'
                    }
                }
       }



    }