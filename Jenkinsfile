node{
  stage('Git Checkout'){
      git url: 'https://github.com/ranjith1428/helloworld.git',
          branch:'master'
  }
  stage('MVN Package'){
    def mvnHome = tool name: 'maven1', type: 'maven'
    sh "${mvnHome}/bin/mvn clean package"
  }
}
