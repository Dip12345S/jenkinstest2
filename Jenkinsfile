pipeline {
    agent any

    parameters {
        string(defaultValue: "", description: "Deployment Name ?", name: "deploymentName")
        choice(choices: ["EU-WEST-2A", "EU-WEST-2B", "EU-WEST-2C"], description: "What AZ ?", name: "azDeploy")
        booleanParam(defaultValue: false, description: "CONFIRM DEPLOYMENT ?", name: "confirmDeploy")
    }
    
    stages {
        stage("deploy") {
            steps{
                echo "Deployment Name : ${deploymentName} \n"
                echo "Select an AZ : ${azDeploy} \n"
                echo "Deployment Confirmation : ${confirmDeploy} \n"
            }
        }
    }
}