node {
    checkout scm
    sh './build.sh'

    if (env.BRANCH_NAME in ['dev','qa','prod']) {
        sh "./deploy.sh ${env.BRANCH_NAME}"
    }
}
