pipeline{
   agent any 

   stages {
    stage ("eb init") {
          steps {
          sh 'eb init ebnodejs -p node.js --region us-east-1 -k Test-teej'
          }          
         }
    stage ("eb use") {
          steps {
          sh 'eb use ebnodejs-dev'
          }         
         }
    stage ("eb deploy") {
          steps {
          sh 'eb deploy --staged'                   
         }
    }

   }
}
