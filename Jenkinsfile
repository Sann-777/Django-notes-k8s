@Library("Shared") _
pipeline {
    agent { label "Vinod" }
    stages {
        stage(hello){
            steps{
                script{
                    hello()
                }
            }
        }
        stage("Clone"){
            steps{
                script{
                    clone("https://github.com/Sann-777/Django-notes-k8s.git","main")
                }
            }
        }
        stage("Build"){
            steps{
                script{
                    docker_build("notes-app", "latest", "asxhazard")
                }
            }
        }
        stage("Push to DockerHub"){
            steps{
                script{
                   docker_push("notes-app", "latest", "asxhazard") 
                }
            }
        }
        stage("Deploy"){
            steps{
                script{
                    docker_compose()
                }
            }
        }
    }
}
