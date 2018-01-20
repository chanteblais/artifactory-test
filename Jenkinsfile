node {
    def server = Artifactory.server artifactory-dev.buffcat.ca

    def uploadSpec = """{
        "files": [
                {
                    "pattern": "my-repository/*",
                    "target": "my_files/"
                }
            ]
        }"""
}
