node('maven'){
stage('maven define'){
   // use the id of the globally configured maven instance
def mvnTool = tool 'Apache Maven 3.6.2'

// execute maven
sh "${mvnTool}/bin/mvn clean package" 
junit allowEmptyResults: true, testResults: 'target/surefire-reports/*.xml'
sh "echo hello world"
   }
//stage('maven package'){
 //  sh "${mvnTool}/bin/mvn clean package"
   // }
stage('3rd stage'){
   sh "echo sample in feature branch "
 }
}
