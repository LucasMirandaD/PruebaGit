pipeline {
   // ------------------------------------
   // -- ETAPA: Compilar
   // ------------------------------------
   stage('build'){
   
   // -- Configura variables
   echo 'Configurando variables'
   def mvnHome = tool 'M3'
   env.PATH = "${mvnHome}\bin:${env.PATH}"
   echo "var mvnHome='${mvnHome}'"
   echo "var env.PATH='${env.PATH}'"
   
   // -- Descarga código desde SCM
   echo 'Descargando código de SCM'
   bat 'rm -rf *'
   checkout scm 
   
   // -- Compilando
   echo 'Compilando aplicacion'
   bat 'mvn clean compile'
}
}