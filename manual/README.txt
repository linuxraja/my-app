The Project created by Maven using the command:

mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

The Main root Content of this project is src, pom.xml & buildspec.yml. Manual folder is just for reference

The code can be built with the command mvn package which was used in buildspec.yml

The build output file will be my-app-1.0.jar 

Prerequisite:

You should create codecommit repo called my-app 
You should have S3 Bucket Created and the relavant bucket should be selected for the destination artifacts 
When you create the build project from AWS Console the Role will be automatically created by Codebuid.The sample poliy Codebuild-allow-S3-commit.json file available for reference


