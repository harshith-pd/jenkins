pipeline{
    agent any
    environment{
        NAME="Harshith"
    }
    stages{
        stage("Greetings"){
            input {
                message '"New Pipeline"'
                ok 'ok'
                submitterParameter 'Pipy'
                parameters {
                    booleanParam defaultValue: true, description: '', name: 'you want it?'
                }
            }

            steps{
                echo "Hello World ${NAME}"
                echo ""${you want it?}
            }  
        }
        stage("Trigger the rest"){
            steps{
                build "Test"
            }
        }
    }
}

