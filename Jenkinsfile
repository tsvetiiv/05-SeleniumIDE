pipeline{
    agent any
    stages{
        stage("Restore the project"){
            steps{
               bat "donet restore"
            }
        }
    
    stage("Build the project"){
        steps{
            bat "donet build --no-restore"
        }
    }
    stage("Run and tests"){
        steps{
            bat "donet test --no-build --verbosity normal"
        }
    }
    }
}