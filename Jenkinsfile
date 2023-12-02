pipeline {
    agent any

    stages {
        stage('Lister les variables') {
            steps {
                script {
                    echo "List of environment variables:"
                    sh 'printenv'
                }
            }
        }

        stage('Utilisation des variables') {
            steps {
                script {
                    // Creating and using environment variables
                    def userName = 'John Doe'
                    def favoriteColor = 'Blue'

                    // Displaying initial values
                    echo "Initial values:"
                    echo "User Name: ${userName}"
                    echo "Favorite Color: ${favoriteColor}"

                    // Creating a new variable describing a hobby
                    def userHobby = 'Reading'

                    // Displaying the initial hobby value
                    echo "User Hobby (Initial): ${userHobby}"

                    // Redefining the favorite color
                    favoriteColor = 'Green'

                    // Displaying updated values
                    echo "Updated values:"
                    echo "User Name: ${userName}"
                    echo "Favorite Color (Updated): ${favoriteColor}"

                    // Redefining the hobby
                    userHobby = 'Gardening'

                    // Displaying the updated hobby value
                    echo "User Hobby (Updated): ${userHobby}"
                }
            }
        }
    }
}

