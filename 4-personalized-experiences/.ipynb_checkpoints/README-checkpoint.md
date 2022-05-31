![banner](static/imgs/MagicMovieMachine_banner.png)
# Building your own movie recommender
This tutorial walks you through building your own movie recommender.
You will see how you can create resources in Amazon Personalize that generate recommendations, just like the Magic Movie Machine!

## Tutorial overview
Completing this tutorial involes the following steps:

1. Follow the instructions in this file to build your environment and find the notebooks in AWS Sagemaker. This involves deploying an AWS CloudFormation stack.
2. Run the `Building_the_Magic_Movie_Machine_Recommender.ipynb` notebook on AWS Sagemaker. 

*Note*: You can explore the notebook directly in github. However, to successfully run it you must follow the steps below to deploy the notebook in a preconfigured environment.

## Building your Environment 
Before you can build your own movie recommender, you must building a work environment as follows:

1. Make sure you have satisfied the environment prerequsites listed below.
2. Deploy the AWS CloudFormation stack.
3. Navigate to the Amazon SageMaker console 

### Environment Prerequisites

To deploy with the CloudFormation template, you must have the following.

1. An AWS Account
2. A user with administrator access to the AWS Account

### Deploying the Environment

The first step is to deploy a CloudFormation template that will perform much of the initial setup for you. In another tab, login to your AWS account. Once you have done that open the link below in a new tab to start the process of deploying the items you need via CloudFormation.

[![Launch Stack](https://s3.amazonaws.com/cloudformation-examples/cloudformation-launch-stack.png)](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=PersonalizeDemo&templateURL=https://amazon-personalize-github-samples.s3.amazonaws.com/PersonalizeDemo.yaml)

Follow along with the screenshots below if you have any questions about these steps.

<details>
  <summary>Click to expand the instructions</summary>
  
### Using the AWS CloudFormation Wizard

Start by clicking `Next` at the bottom like shown:

![StackWizard](static/imgs/img1.png)

In the next page you need to provide a unique S3 bucket name for your file storage, it is recommended to simply add your first name and last name to the end of the default option as shown below, after that update click `Next` again.

![StackWizard2](static/imgs/img3.png)

This page is a bit longer so scroll to the bottom to click `Next`.

![StackWizard3](static/imgs/img4.png)

Again scroll to the bottom, check the box to enable the template to create new IAM resources and then click `Create Stack`.

![StackWizard4](static/imgs/img5.png)

For a few minutes CloudFormation will be creating the resources described above on your behalf it will look like this while it is provisioning:

![StackWizard5](static/imgs/img6.png)

Once it has completed you'll see green text like below indicating that the work has been completed:

![StackWizard5](static/imgs/img7.png)

Now that you have your environment created, you need to save the name of your S3 bucket for future use, you can find it by clicking on the `Outputs` tab and then looking for the resource `S3Bucket`, once you find it copy and paste it to a text file for the time being.


</details>



## Deleting environment resources

Once you have completed all of the work in the Notebooks and have completed the cleanup steps there as well, the last thing to do is to delete the stack you created with CloudFormation. To do that, inside the AWS Console again click the `Services` link at the top, and this time enter in `CloudFormation` and click the link for it.

![StackWizard5](static/imgs/img9.png)

Click the `Delete` button on the demo stack you created:

![StackWizard5](static/imgs/img13.png)

Lastly click the `Delete Stack` button that shows up on the popup:

![StackWizard5](static/imgs/img14.png)

You'll now notice that the stack is in progress of being deleted. Once you see `Delete Completed` you know that everything has been deleted and you are 100% done with this lab.



## Resources

1. Introduction To Amazon Personalize: https://www.youtube.com/c/amazonwebservices/videos
2. Understanding Your Data with Amazon Personalize: https://www.youtube.com/watch?v=TEioktJD1GE
3. Solving Real World Use Cases with Amazon Personalize: https://www.youtube.com/watch?v=9N7s_dVVWBE
4. Getting Your Amazon Personalize Recommendations in Front of Your Users: https://www.youtube.com/watch?v=oeVYCOFNFMI
5. Get Your Amazon Personalize POC to Production: https://www.youtube.com/watch?v=3YawVCO6H14
