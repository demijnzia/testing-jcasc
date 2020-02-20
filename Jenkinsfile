pipeline {
    agent any

    parameters {
        booleanParam(defaultValue: true, description: '', name: 'userFlagged')
    }

    stages {
        stage("foo") {
            steps {
                echo "flag: ${params.userFlag}"
            }
        }
    }
}