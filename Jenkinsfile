pipeline {
    agent { label 'Agent1' }
    
    stages{
        stage('Code'){
            steps{
                git url: 'https://github.com/shahi-farid/node-todo.git', branch: 'master' 
            }
        }
        // stage('Build and Test'){
        //     steps{
        //         sh 'docker build . -t trainwithshubham/node-todo-test:latest'
        //     }
        // }
        // stage('Push'){
        //     steps{
        //         withCredentials([usernamePassword(credentialsId: 'dockerHub', passwordVariable: 'dockerHubPassword', usernameVariable: 'dockerHubUser')]) {
        // 	     sh "docker login -u ${env.dockerHubUser} -p ${env.dockerHubPassword}"
        //          sh 'docker push trainwithshubham/node-todo-test:latest'
        //         }
        //     }
        // }
        // stage('Deploy'){
        //     steps{
        //         sh "docker-compose down && docker-compose up -d"
        //     }
        // }
    }
}
