pipeline {
agent any
stages {
stage('Clone Code') {
steps {
git 'https://github.com/your-repo/simple-devops-project.git'
}
}
stage('Build Docker Image') {
steps {
sh 'docker build -t student-app .'
}
}
stage('Run Container') {
steps {
sh 'docker run -d -p 5000:5000 student-app'
}
}
}
}
