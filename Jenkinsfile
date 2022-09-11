pipeline {
  agent any
  stages {
    stage("Parse YAML") {
      steps {
        script { 
          def datas = readYaml file: 'manifest.yaml'
          for (int i = 0; i < datas.size(); i++) {
            sh "echo Hello ${datas[i]}"
           }
        }
      }
    }
  }
}
