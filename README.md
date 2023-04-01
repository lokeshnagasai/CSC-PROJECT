# CSC-PROJECT
Convert long  url to short url using telegram bot with serverless api using cloud AWS
Use case :
There are several reasons why we might need to convert a long URL into a short one:
Conciseness: Long URLs can be cumbersome to share and remember, especially on platforms that have character limits, such as Twitter. Shortening a URL can make it more concise and easier to share.
Aesthetics: Short URLs can look cleaner and more visually appealing than long URLs, which can be cluttered with random strings of characters.
Tracking: Shortened URLs can be useful for tracking clicks and other analytics. Services that provide URL shortening often offer analytics tools that can show you how many clicks your shortened link has received and where those clicks are coming from.
Security: Some URLs can be very long and complex, and might contain sensitive information such as login credentials or personal details. Shortening the URL can help protect this information by making it less visible and harder to guess.
Overall, shortening URLs can make them more user-friendly, visually appealing, and easier to share, while also providing additional benefits such as tracking and security.

Use of Telegram Bot :
A Telegram bot is an automated software application that runs on the Telegram platform. Bots can interact with users and other bots to perform various tasks, such as answering questions, providing information, sending notifications, and more.

Services used to build this project :

IAM

TELEGRAM BOT

API GATEWAY

LAMBDA

AWS CLOUD WATCH.

IAM :

IAM allows you to create individual user accounts for people within your organization, each with their own set of permissions and access keys. You can also group users together into roles, which allows you to grant permissions to a group of users at once. This makes it easier to manage access to your resources and ensures that users only have access to the resources they need.

API GATEWAY :

API Gateway is a fully managed service provided by Amazon Web Services (AWS) that allows you to create, publish, and manage APIs for your applications. With API Gateway, you can create RESTful APIs, WebSocket APIs, and HTTP APIs to connect to AWS services and other back-end resources.

AWS LAMBDA :

AWS Lambda is a serverless compute service provided by Amazon Web Services (AWS) that allows you to run code without provisioning or managing servers. With Lambda, you can write and run code in response to events, such as changes to data in an S3 bucket, an API Gateway request, or a CloudWatch event.

IMPLEMENTATION :
1.Create a telegram bot using bot father in same
create a unique name for the newly created bot.
3. Note the HTTP API for the given bot and store in note pad.
4. open aws management console and create API using API Gateway
5. select HTTP API and give the api to the request and save
6. create the post method and trigger to lambda after creating the function.
7. Create a lambda function to integrate with api.
8.in api gateway trigger the post method to Lambda to get connected with API.
9.while creating the Lambda function create a role and attach the inline polocy to get interacted with other services manually by giving read and write permissions.
10. Create Iam ->role ->new role -> from lambda -> add inline policy.
In lambda function we have to add our http api and the short url api along with credentials,
create a function that interact with telegram bot input and output message as short url.

heck the logswhether the bot is connected or nor usinf some message.

if its work then your url bot will be worked.
The detailed explaination of code is available in the link :
After connecting the bot check wether it will give the right input or not.
So, the bot is successfully working.
now you can use your own bot for creating short url for imp urls.

LIFE EASY WITH SERVERLESS API IN CLOUD :

Serverless APIs can make certain aspects of life easier by removing the burden of server management and infrastructure maintenance. With serverless APIs, developers can focus on writing code for their application or service without having to worry about scaling, load balancing, or server provisioning.
Serverless APIs also offer the potential for cost savings, as they only require payment for the compute resources used while the API is actually running. Additionally, serverless APIs can be easier to deploy and update, as there is no need to worry about server configuration or downtime during updates.
However, it's important to note that serverless APIs may not be the best solution for all use cases. For applications that require consistent and predictable performance, or that have high computational needs, a serverless architecture may not be the most efficient choice.
Overall, serverless APIs can be a useful tool for developers looking to focus on writing code rather than managing infrastructure, but it's important to carefully evaluate the specific needs of your application before deciding on a serverless architecture.
