pipeline{
    agent any
    stages{
            stage("Git clone"){
                steps{
                    echo 'Git clone'
                    git 'https://github.com/grigciulache/dc.git'
                }
            }
            stage("Build image"){
                steps{
                    echo 'test bild'
                    script {
                            powershell label: '', script: 'docker-compose up -d'
                    }
                }
            }
        
        
    }
}


