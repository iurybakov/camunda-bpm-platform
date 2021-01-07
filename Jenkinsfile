// https://github.com/camunda/jenkins-global-shared-library
// https://github.com/camunda/cambpm-jenkins-shared-library
@Library(['camunda-ci', 'cambpm-jenkins-shared-library']) _

def failedStageTypes = []

pipeline {
  agent none
  stages {
    stage('engine-UNIT-h2') {
      agent {
        node {
          label 'h2'
        }
      }
      steps {
        script {
          def matrices = readYaml('.ci/config/matrices.yaml')
          echo matrices
        }
      }
    }
  }
}
