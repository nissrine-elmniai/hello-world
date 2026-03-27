node {
  try {
    stage('Build') {
      echo 'Compilation du projet...'
      sh 'mvn clean install'
    }
    stage('Test') {
      echo 'Exécution des tests unitaires...'
      sh 'mvn test'
    }
    stage('Deploy') {
      echo 'Déploiement de l\'application...'
      sh 'scp target/app.war user@server:/opt/deploy/'
    }
    echo 'Pipeline terminé avec succès'
  } catch (Exception e) {
    echo "Erreur détectée : ${e}"
    currentBuild.result = 'FAILURE'
  }
}