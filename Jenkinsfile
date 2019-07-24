node('master') {
  try {
    checkout scm
    stage('Initialise') {
      println("Initialised pipeline.")
    }
    stage('Installing node dependencies') {
      echo "npm install"
      sh("npm install")
    }
    stage('Unit testing') {
      echo "npm install"
      sh("npm install")
    }
    stage('Finish') {
        println('Build complete.')
    }
  } catch(err) {
    // currentBuild.result = "FAILED"
    throw err
  } finally {
    echo 'This will always run'
  }
}