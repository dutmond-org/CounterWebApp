node("jnlp") {
  stage('SCM') {
    git 'https://github.com/dutmond-org/CounterWebApp.git'
  }  
  stage('Build') {
    sh 'echo ====hello world===='
  }
  stage('SonarQube analysis') {
    // requires SonarQube Scanner 2.8+
    /** def scannerHome = tool name: 'scanner-3.3.0.1492', type: 'hudson.plugins.sonar.SonarRunnerInstallation';
    withSonarQubeEnv {
      sh "${scannerHome}/bin/sonar-scanner -Dsonar.projectKey=counterwebapp -Dsonar.projectName=CounterWebApp -Dsonar.projectVersion=1.0 -Dsonar.sources=src -Dsonar.language=java -Dsonar.sourceEncoding=UTF-8"
    } */
    sh 'echo =====Running SonarQube======'
  }
    stage('Deploy') {
    sh 'echo ====deploying app===='
  }
}
