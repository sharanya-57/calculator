pipeline {
agent any
stages{
stage('clone'){
git branch:'main',url:'https://github.com/sharanya-57/calculator.git';
}
}
stage('compile'){
steps{
sh'javac Calculator.java'
}
}
stage('build'){
steps{
sh'java Calculator 25 5'
}
}
stage('test'){
steps{
sh'java Calculator 30 5'
}
}
stage('Deploy'){
steps{
echo'Deployement Completed'
}
}
}

