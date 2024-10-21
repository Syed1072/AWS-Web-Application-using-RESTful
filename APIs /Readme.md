Module 4: RESTful APIs with AWS Lambda and Amazon API Gateway In this module you'll use API Gateway to expose the Lambda function you built in the previous module as a RESTful API. This API will be accessible on the public Internet. It will be secured using the Amazon Cognito user pool you created in the User Management module. Using this configuration you will then turn your statically hosted website into a dynamic web application by adding client-side JavaScript that makes AJAX calls to the exposed APIs.

![image](https://github.com/user-attachments/assets/8419e450-1e71-436a-89c3-fa43ced53f4f)

The graph above shows how the Programming interface Passage part you will work in this module coordinates with the current parts you assembled already. The turned gray out things are pieces you have proactively carried out in past advances.

The static site you conveyed in the primary module as of now has a page designed to cooperate with the Programming interface you'll work in this module. The page at/ride.html has a straightforward guide based interface for mentioning a unicorn ride. In the wake of validating utilizing the/signin.html page, your clients will actually want to choose their pickup area by clicking a point on the guide and afterward mentioning a ride by picking the "Solicitation Unicorn" button in the upper right corner.

This module will zero in on the means expected to assemble the cloud parts of the Programming interface, yet assuming you're keen on how the program code functions that calls this Programming interface, you can review the ride.js document of the site. For this situation the application utilizes jQuery's ajax() strategy to make the remote solicitation.

Make Another REST Programming interface Utilize the Amazon Programming interface Passage control center to make another Programming interface named WildRydes.

✅ Bit by bit bearings

Go to the Amazon Programming interface Passage Control center

Pick Make Programming interface.

Select REST, New Programming interface and enter WildRydes for the Programming interface Name.

Select Edge advanced from the Endpoint Type dropdown. Note: Edge streamlined are best for public administrations being gotten to from the Web. Provincial endpoints are ordinarily utilized for APIs that are gotten to fundamentally from inside a similar AWS District. Confidential APIs are for inner administrations within an Amazon VPC.

Pick Make Programming interface

![image](https://github.com/user-attachments/assets/3d6ef30c-f6f6-449b-babb-063cc58d1e57)
