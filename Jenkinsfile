pipeline {
agent any
stages {
stage ("dowork") {
steps {
// do some work
}
}
}
post {
always {
mail to:"buildAdmin@mycompany.com",
subject:"STATUS FOR PROJECT: ${currentBuild.fullDisplayName}",
body: "RESULT: ${currentBuild.result}"
}
}
}
