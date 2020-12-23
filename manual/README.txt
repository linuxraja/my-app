The Project created by Maven using the command:

mvn archetype:generate -DgroupId=com.mycompany.app -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false

The Main root Content of this project is src, pom.xml & buildspec.yml. Manual folder is just for reference

The code can be built with the command mvn package which was used in buildspec.yml

The build output file will be my-app-1.0.jar 

Prerequisite:

You should create codecommit repo called my-app 
You should have S3 Bucket Created and the relavant bucket should be selected for the destination artifacts 
When you create the build project from AWS Console the Role will be automatically created by Codebuid.The sample poliy Codebuild-allow-S3-commit.json file available for reference

You can Download the built file and test the output by the following command (Replace your bucket name)

aws s3 cp s3://check46del/my-app/my-app-1.0.jar .
java -cp my-app-1.0.jar com.mycompany.app.App

cloudwwh.com My First Build!

update the file my-app/src/main/java/com/mycompany/app/App.java and change the Print message, Commit the changes, rebuilt and check the changes 
