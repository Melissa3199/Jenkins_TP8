stage ('build') {
    steps {
        bat 'gradle build'
        archiveArtifacts 'build/libs/*.jar'
    }
    post {
    always {
    echo "Build stage complete" }
    failure {
    echo "Build failed"}
    success {
    echo "Build succeeded" }
    }
}
