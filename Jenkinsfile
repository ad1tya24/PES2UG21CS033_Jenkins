pipeline
{
 agent any
 stages
 {
   stage('Build)
   {
    steps
     {
      build 'PES2UG21CS033-1'
      sh 'g++ text.cpp -o output'
     }
   }
|
stage('Test')
{
steps
{
sh './output'
}
}
stage('Deploy')
{
steps
{
echo 'deploy'
}
}
}

post
{
failure
{
error 'Pipeline failed'
}
}
}
