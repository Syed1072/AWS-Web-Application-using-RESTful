# Wild rydes 
Pause for a minute now and arrangement your Cloud9 improvement climate. ✅ Bit by bit Directions

Go to the AWS The board Control center, click Administrations then, at that point, select Cloud9 under Designer Devices. Click Establish climate. Enter Improvement into Name and alternatively give a Portrayal. Click Following stage. You might leave Climate settings at their defaults of sending off a new t2.micro EC2 occasion which will be stopped following 30 minutes of idleness. Click Subsequent stage. Audit the climate settings and snap Establish climate. It will require a few minutes for your current circumstance to be provisioned and ready. When prepared, your IDE will open to a welcome screen. Underneath that, you ought to see a terminal brief.

You can run AWS CLI orders in here very much like you would on your nearby PC. Check that your client is signed in by running aws sts get-guest character.

``` 
aws sts get-caller-identity
```

You'll see yield demonstrating your record and client data:

```
ec2-user:~/environment $ aws sts get-caller-identity
```

```

{
    "Account": "123456789012",
    "UserId": "AKIAI44QH8DHBEXAMPLE",
    "Arn": "arn:aws:iam::123456789012:user/Alice"
}
```
