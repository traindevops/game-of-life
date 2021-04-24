node {
    stage('git'){
        git 'https://github.com/traindevops/game-of-life.git'
    }
    stage('maven'){
        sh 'mvn clean package'
    }
    stage('archive artifacts'){
        archive 'gaemoflife-web/targets/gameoflife.war'
    }
}
