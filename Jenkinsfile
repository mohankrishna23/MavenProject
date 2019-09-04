node {
stage ('scm checkout'){
git'https://github.com/mohankrishna23/MavenProject.git'
}
stage ('compile-package'){
  def mvnHome = tool name: 'Maven', type: 'maven'
  sh "${mvnHome}/bin/mvn package"
}
}
