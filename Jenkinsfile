pipeline {
  agent any
  stages {
    stage('excute shell') {
      parallel {
        stage('excute shell') {
          agent {
            docker {
              image 'asd'
              args 'asd'
            }

          }
          environment {
            asd = 'asd'
            asdas = 'asd'
          }
          steps {
            sh 'echo "ss" > ll.log'
            sleep(time: 1, unit: 'SECONDS')
          }
        }

        stage('') {
          steps {
            build(job: '12323', propagate: true, wait: true, quietPeriod: 1)
            timestamps() {
              sleep 1
            }

            sleep 1
            retry(count: 1)
            dir(path: 'asdsad')
          }
        }

      }
    }

  }
}