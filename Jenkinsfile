pipeline{
    agent any
    parameters{
        string(name:'Your_Name', defaultValue:'Jarvis',description:'Enter your name')
        text(name:'Role_Name', defaultValue: '', description:'Your role')
        choice(name:'Release', choices:['alpha','beta','final'], description:'Enter the release')
        booleanParam(name:'Agree',defaultValue:true, description: 'Are the above details true?')
        password(name: 'PASSWORD', defaultValue: 'nothing', description: 'Enter a password')
    }
    stages{
        stage('Param Example'){
            steps{
                echo "Hello ${params.Your_Name}"

                echo "Role: ${params.Role_Name}"

                echo "Agree?: ${params.Agree}"

                echo "Choice: ${params.Release}"

                echo "Password: ${params.PASSWORD}"
                
            }
        }
    }
}
