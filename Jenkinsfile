node { // <1>
    stage('Build') {
        echo 'Starting build phase'
        sh 'npm install'
    }
    stage('Test') {
        echo 'Starting test phase'
        MOCHA_FILE=./jenkins-test-results.xml mocha --reporter mocha-junit-reporter
    }
    stage('Deploy') {
        /* .. snip .. */
    }
}