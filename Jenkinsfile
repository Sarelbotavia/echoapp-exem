pipeline{
    agent any
    // tools{
    // }
    stages{
        stage("build"){
            steps{
                echo '========================= Executing Build Stage =========================================='
                sh 'ls -R'
                dir("./echo"){
                    sh 'docker build -t app .'
                    echo 'Verify success!!!!!!!!!!!!!!!!!!!!!!!!!!!!'
                }
            }
        }
        // stage("test1"){
        //     steps{
        //         echo '========================== Executing test1 Stage ======================================='
        //         sh 'curl app:9191'
        //     }
        // stage("getGitCommit"){
        //     steps{
        //         env.GIT_COMMIT_MSG = sh (script: 'git log -1 --pretty=%B ${GIT_COMMIT}', returnStdout: true).trim()
        //     }
        // }
        // stage("deploy"){
        //     when{
        //         expression { BRANCH_NAME =~ /^(master)/ || (env.GIT_COMMIT_MSG=~ /(#test)/ && BRANCH_NAME =~ /^(feature)/)}
        //     }
        //     steps{
        //         script {
        //             echo '======================== Executing deploy Stage ========================================='
        //             if (BRANCH_NAME =~ /^(feature)/){

        //             }
        //             else{

        //             }
        //         }
        //     }           
        // }
    }
    // post {
    //     always {
    //         script { 
    //             sh ''
    //         }
    //     }
    //     failure {
    //         script {
    //             sh ''
    //         }
    //     }
    //     changed {
    //         sh 'echo "sendEmail(sarelb1986@gmail.com)"'
    //     }
    // }
}