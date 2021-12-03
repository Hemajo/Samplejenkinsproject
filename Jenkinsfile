node{
    stage ("SCM Checkout"){
        git branch: 'main', url: 'https://github.com/Hemajo/Samplejenkinsproject.git'
    }
    stage ("Installing and starting apache"){
        sh 'sudo apt-get install apache2 -y'
        sh 'sudo service apache2 start'
    }
    stage ("Deploying"){
        sh 'sudo cp -R * /var/www/html/'
    }
}