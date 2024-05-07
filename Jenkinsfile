pipeline{
agent {label "agentfarm" }
stages {
stage('Delete the workspace'){
steps{
cleanWs()
}
}
stage('Installing Java and Maven') {
steps {
sh 'sudo apt-get update -y && sudo apt-get upgrade -y'
sh 'sudo apt install -y wget tree unzip openjdk-11-jdk maven'
sh 'mvn -version'
}
}
stage('Third Stage'){
steps {
echo "Third Stage"
}
}
}
}
