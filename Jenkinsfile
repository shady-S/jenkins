pipeline {
agent any
stages {
stage ('Compile Stage') {
steps {
 withMaven{
sh'mvn clean compile'
}
}
}
stage ('Testing Stage') {
steps {
withMaven() {
bat'mvn test'
}
}
}
stage ('Install Stage') {
steps {
withMaven() {
bat'mvn install'
}
}
}
}
}
