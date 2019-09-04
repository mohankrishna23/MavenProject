node {
  try {
stage ('scm checkout'){
git'https://github.com/mohankrishna23/MavenProject.git'
}
stage ('compile-package'){
  def mvnHome = tool name: 'Maven', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
}
  }
  catch(err) {
        println(err.toString())
        error(err.getMessage())
    }
  finally {
        stage('Clean up') {
            cleanWs()
        }
}
