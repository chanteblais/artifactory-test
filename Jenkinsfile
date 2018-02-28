def server = Artifactory.server "artifact01"
def uploadSpec

node (label: 'jbuild01_docker') {

    stage('Clone repository') {

        checkout scm
    }
    
    stage('Upload') {
        
        uploadSpec = """{
          "files": [
            {
              "pattern": "/home/build/workspace/Artifactory_Push_Test_CB/files/",
              "target": "my-repository"
            }
         ]
        }""" 
        
        server.upload(uploadSpec)
    }
}
