What is Amazon Lex?

Amazon Lex is a service for building conversational interfaces using voice and text. Powered by the same conversational engine as Alexa, Amazon Lex provides high quality speech recognition and language understanding capabilities, enabling addition of sophisticated, natural language ‘chatbots’ to new and existing applications. Amazon Lex reduces multi-platform development effort, allowing you to easily publish your speech or text chatbots to mobile devices and multiple chat services, like Facebook Messenger, Slack, Kik, or Twilio SMS. Native interoperability with AWS Lambda and Amazon CloudWatch and easy integration with many other services on the AWS platform including Amazon Cognito, and Amazon DynamoDB makes bot development effortless.
Q: How can I get started with Amazon Lex?

To start using Amazon Lex, simply sign into the AWS Management Console and navigate to “Lex” under the “Artificial Intelligence” category. You must have an Amazon Web Services account to start using Amazon Lex. If you do not already have one, you will be prompted to create one during the sign-up process. Please refer to the Amazon Lex V2 Getting Started Guide for more information.
Q: What are the most common use cases for Amazon Lex?

The most common use-cases include:
Self-service voice assistants and chatbots – build a call center bot
Informational bot – build an automated customer support agent or bot that answers questions
Application/Transactional bot – build a stand-alone pizza ordering agent or a travel bot
Enterprise Productivity bot – build custom bots to connect to enterprise data resources
Device Control bot– use Amazon Lex to issue control commands to connected devices
Q: How does Amazon Lex work with other AWS services?

Amazon Lex leverages AWS Lambda for Intent fulfillment, Amazon Cognito for user authentication, and Amazon Polly for text to speech.
Q: Do I have to be a machine learning expert to use Amazon Lex?

No machine learning expertise is necessary to use Amazon Lex. Developers can declaratively specify the conversation flow and Amazon Lex will take care of the speech recognition and natural language understanding functionality. Developers provide some sample utterances in plain English and the different parameters (slots) that they would like to collect from their user with the corresponding prompts. The language model gets built automatically.
Q: In which AWS regions is Amazon Lex available?

For a list of the supported Amazon Lex AWS regions, please visit the AWS Region Table for all AWS global infrastructure. Also for more information, see Regions and Endpoints in the AWS General Reference.
Q. What is the maximum bandwidth supported on Amazon Lex?

Amazon Lex scales to your needs and does not impose bandwidth constraints.
Q: Is Amazon Lex a managed service?

Amazon Lex is a completely managed service so you don’t have to manage scaling of resources or maintenance of code. Your interaction schema and language models are automatically backed up. We also provide comprehensive versioning capability for easy rollback. Amazon Lex architecture does not require storage or backups of end user data.
Q: When do I use Amazon Polly vs. Amazon Lex?

Amazon Polly converts text inputs to speech. Amazon Lex is a service for building conversational interfaces using voice and text.
Q: Does Amazon Lex get more intelligent over time?

Yes. Amazon Lex uses deep learning to improve over time.
Bot Structure
Q: How do I create a bot in Amazon Lex?

To create a bot, you will first define the actions performed by the bot. These actions are the intents that need to be fulfilled by the bot. For each intent, you will add sample utterances and slots. Utterances are phrases that invoke the intent. Slots are input data required to fulfill the intent. Lastly, you will provide the business logic necessary to execute the action. An Amazon Lex bot can be created both via Console and REST APIs.
Q: Can I implement business logic on the client?

Yes. Amazon Lex provides the option of returning parsed intent and slots back to the client for business logic implementation.
Q: How can I validate user input?

Amazon Lex provides deep integration with AWS Lambda and you can validate user input using the initialization and validation codeHook. This code gets executed at every turn of the conversation. The codehook can be used to set up session parameters, validate user input and customize responses.
Q: What is an Intent?

To build an Amazon Lex bot, you will need to identify a set of actions - known as 'intents’ -- that you want your bot to fulfill. A bot can have multiple intents. For example, a ‘BookTickets’ bot can have intents to make reservations, cancel reservations and review reservations.
Q: What is an utterance?

An ‘utterance’ is the spoken or typed phrase to invoke an intent. For example, to invoke the intent to make reservations, you would provide a sample utterance such as, “Can I make a reservation?”
Q: What are slots?

To fulfill an intent, the Amazon Lex bot needs information from the user. This information is captured in ‘slots’. For example, you would define show name and time as slots for intent to make reservations.
Q: What are prompts?

Amazon Lex elicits the defined ‘slots’ by using the ‘prompts’ provided. For example, to elicit value for the slot ‘time’ you will define a prompt such as “What show time would you like to reserve?”. Amazon Lex is capable of eliciting multiple slot values via a multi-turn conversation.
Q: How is an action fulfilled?

Amazon Lex integrates with AWS Lambda for ‘fulfillment’ of the action or business logic. Alternately, you can configure Amazon Lex to return parsed intent and slot values to the client for action fulfillment.
Q: How do I monitor and track my bot?

You can track metrics for your bot on the ‘Monitoring’ dashboard in the Amazon Lex Console. Currently, you can track the number of missed utterances, request latency and traffic by channel for your bot. You can view list of utterances that were not recognized by your bot, aka 'missed utterances'. With these monitoring capabilities, you view how your users are interacting with the bot and make improvements over time.
