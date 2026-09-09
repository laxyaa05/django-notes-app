@Library("shared") _
pipeline{
    agent { label "laxyaa" }
    triggers { githubPush() }
    stages{
        stage("hello"){
            steps{
                script{
                    hello()
                }
            }
        }
        stage("Code"){
            steps{
                script{
                   clone("https://github.com/LondheShubham153/django-notes-app.git","main") 
                }
            }
        }
        stage("Build"){
            steps{
                script{
                    build()
                }
            }
        }
        stage("Deploy"){
            steps{
                script{
                    deploy()
                }
            }
        }
    }
}
