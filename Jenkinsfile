pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Building project...'
                sh 'ls'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                sh '''
                python3 - <<EOF
import calculator

print('Testing add:', calculator.add(2,3))
print('Testing sub:', calculator.sub(5,2))
print('Testing mul:', calculator.mul(3,4))
print('Testing div:', calculator.div(10,2))
EOF
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage (dummy)...'
            }
        }
    }
}
