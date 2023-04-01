pipeline {
    agent any

    stages {
        stage('Deploy PHP applicaiton') {
            steps {
                sshPublisher(publishers: [sshPublisherDesc(configName: 'staging.ems-ce.com', transfers: [sshTransfer(cleanRemote: false, excludes: '', execCommand: '', execTimeout: 120000, flatten: false, makeEmptyDirs: false, noDefaultExcludes: false, patternSeparator: '[, ]+', remoteDirectory: '/var/www/staging.ems-ce.com/', remoteDirectorySDF: false, removePrefix: '', sourceFiles: '**/*.*')], usePromotionTimestamp: false, useWorkspaceInPromotion: false, verbose: false)])
            }
        }
    }
}
