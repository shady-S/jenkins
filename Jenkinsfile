pipeline {
agent any
   tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "maven"
   }
stages {
stage ('Compile Stage') {
steps {
 withMaven{
bat'mvn clean compile'
}
}
}
stage ('Testing Stage') {
steps {
withMaven {
bat'mvn test'
}
}
}
stage ('Install Stage') {
steps {
withMaven {
bat'mvn install'
}
}
}
}
}
