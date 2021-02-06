pipeline{
    agent any
    stages{
        stage("Thamu's checkout"){
            steps{
             checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/thamunkpillai/webapplication.git']]])
            }
        }
        stage("testing"){
            steps{
                echo "am testing"
            }
        }
        stage("deploy"){
            steps{
                echo "Deploying code"
            }
        }
    }
}



