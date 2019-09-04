node {
stage ('scm checkout'){
git'https://github.com/mohankrishna23/MavenProject.git'
}
stage ('compile-package'){
sh 'mvn package'
}
}
