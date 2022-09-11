pipeline {
  agent any
  stages {
    stage("Parse YAML") {
      steps {
        script { 
          def datas = readYaml file: 'manifest.yaml'
          echo '${datas}'
        }
      }
    }
  }
}
