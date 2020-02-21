pipeline {
    agent any

    parameters {
        text(defaultValue: '', description: 'DSA debug mode values.', name: 'DSA_DEBUG_PARAM')
        string(defaultValue: '', description: 'e.g. #automation-fips<br>No value means not sending results to any channel.', name: 'SLACK_CHANNEL')
        choice(choices: ['Enable, 'Disable'], description: '', name: 'COCO_MODE')
    }

    stages {
        stage("foo") {
            steps {
                echo "SLACK_CHANNEL: ${params.SLACK_CHANNEL}"
                echo "COCO_MODE: ${params.COCO_MODE}"
            }
        }
    }
}