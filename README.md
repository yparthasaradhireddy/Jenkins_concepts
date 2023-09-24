# Jenkins_concepts
## Global Variable Reference: 
The Variable are built in Jenkins. We have 3 types of  Global variables
1)	Env: env.PATH or env.BUILD_ID. 
2)	Params: params.MY_PARAM_NAME.
3)	currentBuild: currentBuild.result, currentBuild.displayName, etc.
   
## environment variables:
• BUILD_ID <br>
•	BUILD_NUMBER <br>
•	BUILD_TAG <br>
•	BUILD_URL <br>
•	EXECUTOR_NUMBER <br>
•	JAVA_HOME <br>
•	JENKINS_URL <br>
•	JOB_NAME <br>
•	NODE_NAME <br>
•	WORKSPACE <br>

## Restarting from the Classic UI: <br>
Once your Pipeline has completed, whether it succeeds or fails, you can go to the side panel for the run in the classic UI and click on "Restart from Stage". <br>
You will be prompted to choose from a list of top-level stages that were executed in the original run, in the order they were executed. Stages which were skipped due to an earlier failure will not be available to be restarted, but stages which were skipped due to a when condition not being satisfied will be available. The parent stage for a group of parallel stages, or a group of nested stages to be run sequentially will also not be available - only top-level stages are allowed.
    
## Customizing the execution environment: (Docker): <br>

Pipeline is designed to easily use Docker images as the execution environment for a single Stage or the entire Pipeline. Meaning that a user can define the tools required for their Pipeline, without having to manually configure agents. Any tool that can be packaged in a Docker container can be used with ease, by making only minor edits to a Jenkinsfile.




