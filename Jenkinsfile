pipeline
{
agent any
stages
{
 
stage('scm ceckout')
{ steps { sh 'echo code_downloading'}}

stage ('testing')
 {parallel 
    { stage ('unit testing')
      { steps {sh 'echo unit_testing'} }
     
    { stage ('integration testing')
      { steps {sh 'echo integration_testing'} }

     stage ('component testing')
      { steps {sh 'echo component_testing'} } }

   }

}
}
