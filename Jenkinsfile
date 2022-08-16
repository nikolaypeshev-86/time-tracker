node {
stage('SCM')

{ git 'https://github.com/nikolaypeshev-86/time-tracker.git' }
stage('SonarQube Analysis') {
//def mvn = tool 'local-maven3.8.2';
// withSonarQubeEnv(credentialsId: 'sqp_c1fefcba402ef32cb7a7d35adffac4bf3588559e',installationName: 'sq1')

{ sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Jenkins -Dsonar.host.url=http://bgsovm00017.corp.polygran.de:9000 -Dsonar.login=sqp_88f9f42107e3bb5a5d02ef93d5b519855958434b' // }
}
}
