stage('Test') {
    steps {
        echo 'Running tests...'
        sh '''
        python3 - <<EOF
import calculator

assert calculator.add(2,3) == 5, "Add function is incorrect!"
assert calculator.sub(5,2) == 3, "Sub function is incorrect!"
assert calculator.mul(3,4) == 12, "Mul function is incorrect!"
assert calculator.div(10,2) == 5, "Div function is incorrect!"

print("All tests passed!")
EOF
        '''
    }
}
