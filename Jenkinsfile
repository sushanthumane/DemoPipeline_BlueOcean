pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'step 1 from stage 1'
      }
    }

    stage('Stage2') {
      parallel {
        stage('Stage2') {
          steps {
            echo 'step 1from Statg2 '
          }
        }

        stage('Stage3') {
          steps {
            echo 'Stage 2 step 2'
          }
        }

      }
    }

    stage('Stage4') {
      steps {
        echo 'stage4 step1'
      }
    }

  }
}