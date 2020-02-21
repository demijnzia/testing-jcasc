pipeline {
    agent any

    parameters {
        string(defaultValue: '', description: 'The Testrail Test Plan ID to send the results to.<br>No value means not sending results to Testrail.', name: 'TESTRAIL_PLANID')
        string(defaultValue: '3', description: '# of hours before VM is removed.', name: 'VM_EXPIRED_HOUR')
        booleanParam(defaultValue: false, description: 'Enable or disable FIPS mode for DSM.', name: 'DSM_FIPS_MODE')
        booleanParam(defaultValue: false, description: 'Enable or disable FIPS mode for DSA.', name: 'DSA_FIPS_MODE')
        text(defaultValue: '', description: 'DSA debug mode values.', name: 'DSA_DEBUG_PARAM')
        string(defaultValue: '', description: 'e.g. #automation-fips<br>No value means not sending results to any channel.', name: 'SLACK_CHANNEL')
        choice(choices: ['Enable', 'Disable'], description: '', name: 'COCO_MODE')
    }

    stages {
        stage("foo") {
            steps {
                echo "TESTRAIL_PLANID: ${params.TESTRAIL_PLANID}"
                echo "VM_EXPIRED_HOUR: ${params.VM_EXPIRED_HOUR}"
                echo "DSM_FIPS_MODE: ${params.DSM_FIPS_MODE}"
                echo "DSA_FIPS_MODE: ${params.DSA_FIPS_MODE}"
                echo "DSA_DEBUG_PARAM: ${params.DSA_DEBUG_PARAM}"
                echo "SLACK_CHANNEL: ${params.SLACK_CHANNEL}"
                echo "COCO_MODE: ${params.COCO_MODE}"
            }
        }
    }
}