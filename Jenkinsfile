pipeline {
  agent any
  stages {
    stage('Update Feeds') {
      steps {
        sh '''./scripts/feeds update -a 
./scripts/feeds install -a 

make deflinino
make tools/install V=99 && make toolchain/install V=99'''
      }
    }
  }
}