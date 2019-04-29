node("jnlp") {
  stage('SCM') {
    git 'https://github.com/dutmond-org/CounterWebApp.git'
  }
  stage('SonarQube analysis') {
    // requires SonarQube Scanner 2.8+
    def scannerHome = tool name: 'scanner-3.3.0.1492', type: 'hudson.plugins.sonar.SonarRunnerInstallation';
    withSonarQubeEnv {
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}

