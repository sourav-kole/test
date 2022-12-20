node {
    stage('Checkout ropository') {
        git branch: 'main', url: 'https://github.com/sourav-kole/test.git'
    }

    stage('Install node modules') {
        bat "npm install"
    }

    stage('Build') {
        bat "npm run-script build --prod"
    }

    stage('Deploy') {
        bat("move dist\\test\\*.* C:\\Apache24\\htdocs")
    }
}