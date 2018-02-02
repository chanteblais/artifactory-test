def server = Artifactory.server "artifact01"
def downloadSpec = """{
    "files": [
          {
              "pattern": my-repository/test/,
              "target": "bazinga/"
            }
          ]
        }""" 

pipeline {
    agent { 
        label 'SlaveNode' 
    }
    stages {
        stage('Example') {
            steps {
            }  
        }
    }
}
