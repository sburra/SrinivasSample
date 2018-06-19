 node('windows') {
        checkout scm
        try {
            unstash 'app'
            bat 'make check'
        }
        finally {
            junit '**/target/*.xml'
        }
    }