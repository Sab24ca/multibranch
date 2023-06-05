pipeline
{
    agent any
    stages
    {
        stage('ContDownload')
        {
            steps
            {
                script
                {
                    try
                    {
                        git 'https://github.com/Sab24ca/maven10.git'
                    }
                    catch(Exception e1)
                    {
                       mail bcc: '', body: 'Jenkins is unable to download dev code from github', cc: '', from: '', replyTo: '', subject: 'Download Failed', to: 'git.admin@gmail.com'
                       exit(1)
                    }
                 }
             }
         }
     }
}         
