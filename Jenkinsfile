pipeline {
   agent any
    parameters {
        choice(name: "Environment", choices:["Preprod","Prod","staging"])
        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')
    }
   stages {
      stage('Hello') {
         steps {
            sh 'python3 --version'
            sh 'echo "lets see!"'
	    sh "bash harry.sh"
         script {
             def browsers=["chrome", "firefox"]
             for (int i=0; i<browsers.size();i++) {
                 echo "testing the ${browsers[i]}"
             }
         }
         }
      }
   }
}

