pipeline {
    
agent { node { label 'master' } } 
parameters {
        string(name: 'FileName', defaultValue: '', description: 'Pls supply filename')
}
stages {
   stage('Read demo file') {
            steps {
                // sh is for shell command
                // sh 'cat demo.txt'  // without parameter - use single quote
                // with parameter - use double coute, $sign for the params and parentesis 
                sh "cat ${params.FileName}"
            }
        }
        // second stage directives
    stage('Read Readme.md file') {
            steps{
            sh 'cat README.md'
        }
    }
     
    }
}   

