**Module 1: Static Web Hosting with AWS Amplify Console**

In this module you'll configure AWS Amplify Console to host the static resources for your web application. In subsequent modules you'll add dynamic functionality to these pages using JavaScript to call remote RESTful APIs built with AWS Lambda and Amazon API Gateway.

Architecture Overview
![image](https://github.com/user-attachments/assets/4b06d6d8-6a0b-473f-b4ee-1195fad1cf34)

You'll see yield showing your record and client data: Guarantee you've finished the arrangement guide prior to starting the studio.

Every one of the accompanying segments gives an execution outline and definite, bit by bit guidelines. The outline ought to give sufficient setting to you to finish the execution on the off chance that you're as of now acquainted with the AWS The executives Control center or you need to investigate the administrations yourself without following a walkthrough.

Locale Choice This studio step can be conveyed in any AWS district that upholds the accompanying administrations:

AWS Enhance Control center AWS CodeCommit You can allude to the AWS area table in the AWS documentation to see what locales have the upheld administrations. Among the upheld locales you can pick are:

North America: N. Virginia, Ohio, Oregon Europe: Ireland, London, Frankfurt Asia Pacific: Tokyo, Seoul, Singapore, Sydney, Mumbai Whenever you've picked a locale, you ought to send each of the assets for this studio there. Ensure you select your district from the dropdown in the upper right corner of the AWS Control center prior to getting everything rolling.

Locale determination screen capture

Make the git vault You have two choices for this initial step which is to either utilize AWS CodeCommit or GitHub to have your site's vault. The decision is yours. In the event that you have a GitHub account go ahead and utilize that. In any case CodeCommit is remembered for the AWS Complementary plan

Utilizing CodeCommit The AWS Cloud9 improvement climate accompanies AWS oversaw transitory accreditations that are related with your IAM client. You utilize these qualifications with the AWS CLI certification assistant. Empower the qualification aide by running the accompanying two orders in the terminal of your Cloud9 climate.

git config - - worldwide credential.helper '!aws codecommit qualification aide $@' git config - - worldwide credential.UseHttpPath valid Next you want to make the storehouse and clone it to your Cloud9 climate:

Open the AWS CodeCommit console Select Make Archive Set the Archive name* to "wildrydes-site" Select Make From the Clone URL drop down, select Clone HTTPS Presently from your Cloud9 improvement climate:

From a terminal window run git clone and the HTTPS URL of the respository: ec2-user:/climate $ git clone https://git-codecommit.us-east-1.amazonaws.com/v1/repos/wildrydes-site Cloning into 'wildrydes-site'... caution: You seem to have cloned an unfilled vault. ec2-user:/climate $ Extra Github Step (This step is possibly required on the off chance that you're utilizing Github rather than Codecommit) ✅ Bit by bit headings

Adhere to the directions on GitHub to Make a storehouse. NOTE: You shouldn't make a first commit, simply make the store. Clone the vault locally utilizing your GitHub qualifications On the off chance that you don't have credentially locally, or need to involve Cloud9 for the present lab, follow these moves toward Creating another SSH key and adding it to the ssh-specialist Clone the archive Populate the git archive When your git archive is made and cloned locally, you'll have to pull in the records for your site and sync them up to the vault.

```
$ git add .
$ git config --global user.email "<EMAIL ADDRESS>"
$ git config --global user.name "<USER NAME>"
$ git commit -m "initial checkin of website code"
$ git push

Username for 'https://git-codecommit.us-east-1.amazonaws.com': wildrydes-codecommit-at-xxxxxxxxx
Password for 'https://wildrydes-codecommit-at-xxxxxxxxx@git-codecommit.us-east-1.amazonaws.com': 
Counting objects: 95, done.
Compressing objects: 100% (94/94), done.
Writing objects: 100% (95/95), 9.44 MiB | 14.87 MiB/s, done.
Total 95 (delta 2), reused 0 (delta 0)
To https://git-codecommit.us-east-1.amazonaws.com/v1/repos/wildrydes-site
 * [new branch]      master -> master
```
✅ Bit by bit bearings From your Cloud9 advancement environment(or nearby climate)
