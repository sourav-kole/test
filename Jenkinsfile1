node {
    stage('Checkout ropository') {
        git branch: 'main', url: 'https://github.com/sourav-kole/test.git'
    }

    stage('Install node modules') {
        sh "npm install"
    }

    stage('Build') {
        sh "npm run-script build --prod"
    }
}