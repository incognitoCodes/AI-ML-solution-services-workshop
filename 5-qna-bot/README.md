# AWS QnABot

AWS QnABot is a multi-channel, multi-language conversational interface (chatbot) that responds to your customer’s questions, answers, and feedback. The solution allows you to deploy a fully functional chatbot across multiple channels including chat, voice, SMS and Amazon Alexa. 

## What you will learn?
This demo is designed to cover the initial set up of the AWS QnABot and explore some of it's core features. This demo will cover the following:

- Deploying the AWS QnABot in your AWS account
- Populating the chatbot with your questions and answers
  - Enriching your answers with images, plaintext, rich text, and SSML
  - Supporting follow-up questions and contextual user journeys
- Asking questions using voice or text chat
- Integrating the solution with Amazon Kendra to find answers from unstructured documents
- Enabling multi-language support for different user requirements
- Monitoring the solution’s usage and user feedback through a Kibana dashboard

**AI Services used**
- [Amazon Lex](https://aws.amazon.com/lex/)
- [Amazon Transcribe](https://aws.amazon.com/transcribe/)
- [Amazon Translate](https://aws.amazon.com/translate/)
- [Amazon Polly](https://aws.amazon.com/polly/)
- [Amazon Kendra](https://aws.amazon.com/kendra/)
- [Amazon Comprehend](https://aws.amazon.com/comprehend/)

**The most common use-cases for QnA Chatbot include:**
- Chatbot for the website, or mobile apps.
- Integration with call centre to improve and automate operations.
- Ask questions using the latest Amazon Echo devices
- Measure ad monitor the solution’s usage and user feedback
- Enterprise search through QnA chatbot with Amazon Kendra to find answers from unstructured documents
- Integrate the solution with Amazon Connect to provide automation for your call center

## How to get started
This demo is not designed to be followed along in real time, however we encourage you to deploy the QnA Bot in your workshop account to explore the solution separately. This deployment will take approx. 30 - 45 mins to deploy. 

### Pre-requisites 
- Ensure you are in us-east-1. 

### 1) Deploy the QnABot solution 
- To deploy the QnABot solution follow the deployment instructions [here](https://docs.aws.amazon.com/solutions/latest/qnabot-on-aws/automated-deployment.html). 

### 2) Populate your chat bot with questions and answers

*Access your Content Designer* 
- Once your QnABot has finished deploying, navigate to the cloudformation service in the AWS Console. 
- Select 'Stacks'
- Select the Stack name you chose in section 1 of these instructions. 
- Select 'Outputs' 
This is where all of the resources associated with your AWS QnABot is located. 

*To create questions and answers in the content designer:*
- Follow the instructions [here](https://catalog.us-east-1.prod.workshops.aws/workshops/20c56f9e-9c0a-4174-a661-9f40d9f063ac/en-US/qna/questions) 

*To enable your QnA Bot to elicit questions:* 
-  Follow the instructions [here](https://catalog.us-east-1.prod.workshops.aws/workshops/20c56f9e-9c0a-4174-a661-9f40d9f063ac/en-US/qna/elicit-response) 
 
*To create guided user journeys*
- Follow the instructions [here](https://catalog.us-east-1.prod.workshops.aws/workshops/20c56f9e-9c0a-4174-a661-9f40d9f063ac/en-US/qna/guided-navigation) 

### 3) Ask questions using Voice or Text and use multiple languages 
*To enable users to be able to ask questions by voice*
- This is auto-enabled! Just click the microphone in the Client URL. 

*To enable multiple languages* 
- Follow the instructions [here](https://docs.aws.amazon.com/solutions/latest/qnabot-on-aws/automatic-translation.html)

### 4) Amazon Kendra
*To enable Amazon Kendra*
- Follow the Instructions [here](https://docs.aws.amazon.com/solutions/latest/qnabot-on-aws/integrate-amazon-kendra.html)

### 5) Kibana Dashboard
*To access the Kibana Dashboard and to learn how to use it to tune your QnABot*
- Follow the Instructions [here](https://catalog.us-east-1.prod.workshops.aws/workshops/20c56f9e-9c0a-4174-a661-9f40d9f063ac/en-US/tuning/tuning) 

## Next Steps
The QnA Bot code is available for your review and customizations. You can use this simple solution to build your own QnA Bot rapidly and integrate it to your existing website easily. Please see the resources below to explore how you can integrate other tools such as Amazon Connect, and Alexa.

Speak to your AWS Account Manager if you wish to discuss your use case further.

## Resources
- Blog - [Building an omnichannel Q&A chatbot](https://aws.amazon.com/blogs/machine-learning/building-a-multi-channel-qa-chatbot-with-amazon-connect-amazon-lex-amazon-kendra-and-the-open-source-qnabot-project/)
- Blog - [Create a Question and Answer Bot with Amazon Lex and Amazon Alexa](https://aws.amazon.com/blogs/machine-learning/creating-a-question-and-answer-bot-with-amazon-lex-and-amazon-alexa/)
- Blog - [Deploy a Web UI for Your Chatbot](https://aws.amazon.com/blogs/machine-learning/deploy-a-web-ui-for-your-chatbot/)
- [Solution](https://aws.amazon.com/solutions/implementations/aws-qnabot/)
- [Workshop](https://catalog.us-east-1.prod.workshops.aws/v2/workshops/20c56f9e-9c0a-4174-a661-9f40d9f063ac/)
- [Kendra Index Tutorial](https://aws.amazon.com/getting-started/hands-on/create-query-index-with-amazon-kendra/)
