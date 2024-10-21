Serverless GraphQL API Note! This section is currently part of expansion of this lab. There is currently no Step 7

In this module you'll use AWS AppSync to build a GraphQL API to find more information about the rides you have taken so far. In a subsequent module you will then modify our web application to add the ride history page which will query this API.

Architecture Overview In the [Serverless Backend][serverless-backend] module you created a Lambda function that stored data in a DynamoDB bucket. Then in the RESTful APIs module you put Amazon API Gatewway infront of the Lambda function so you could connect it to your web application. Every time that you request a ride through that API, the Lambda function stores the data. Now, let's get that data out and present it as ride history.

GraphQL provides a robust query language API that works well with web and mobile based applications. AWS AppSync has the ability to put a GraphQL API infront of many different backends, including: AWS DynamoDB, AWS ElasticSearch Service, Amazon RDS Aurora, and AWS Lambda functions. The GraphQL API you will build here will allow you to return all rides, information about rides by their ID, and information about the unicorns that served your ride.

![image](https://github.com/user-attachments/assets/34ca90ef-4af0-4a5e-b39b-7aafbc1de2e6)

Make an AppSync GraphQL Programming interface Undeniable Level Directions Utilize the AWS AppSync control center to make another GraphQL Programming interface. Call your Programming interface RidesHistory. Import the DynamoDB data set made in the [Serverless Backend][serverless-backend] module and afterward make an extra question for getting all rides by a specific unicorn.

✅ Bit by bit headings

Go to the AWS AppSync Control center.

Pick Make Programming interface.

Select Import DynamoDB table and snap Start.

Select the Locale of your table and enter its Table name. Leave New Job chose. Click Import.

![image](https://github.com/user-attachments/assets/02713cf4-db04-4636-bf58-c4dacb0d4303)

AppSync will just distinguish the Essential Key which was set for your DynamoDB table, yet you'll need to plan the other information saved by the Lambda capability for each ride. You can find what the fields are by checking out at a thing from your table:

Go to the Amazon DymamoDB console in another program tab or window. From the left route, select Tables. Select the table you made before (it ought to be Rides). Select the Things tab and afterward select a ride by its RideId. In the spring up window that opens, select Text and really look at DynamoDB JSON. Record the JSON made here into a scratchpad so you can allude to it later. The JSON contains the trait name, type, and information. Select Drop to close the popup without changing the thing. Back in the AppSync console, arrange the information model by adding fields that address all off the high level thing ascribes recorded from DynamoDB. The things with type S are Strings, M are JSON Article, Exhibit, or Worth. Really look at the container for Expected for all records.

![image](https://github.com/user-attachments/assets/3e9caad9-01b4-4862-a362-4d2c04afeef7)

Click Create.

Name the API RidesHistory and click Create.
