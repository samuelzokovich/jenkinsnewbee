pipeline {
  agent any
  stages {
    stage("Parse YAML") {
      steps {
        script { 
            datas = readYaml (file: 'manifest.yml')
            echo datas.ear_file.deploy.toString()
        }
      }
    }
  }
}
