## Getting Started with Liquid to Customize the Looker User Experience

https://github.com/quiccklabs/Labs_solutions/blob/93abaca8d03739f5e12008661387e16aa6f3a704/Getting%20Started%20with%20Liquid%20to%20Customize%20the%20Looker%20User%20Experience



## Getting Started with Security Command Center
```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Getting%20Started%20with%20Security%20Command%20Center/quicklabgsp1124.sh

sudo chmod +x quicklabgsp1124.sh

./quicklabgsp1124.sh
```

## Redacting Sensitive Data with Cloud Data Loss Prevention

perform mnaually that will be faster
```cmd
gcloud config set compute/region us-west1
git clone https://github.com/googleapis/synthtool
cd synthtool/tests/fixtures/nodejs-dlp/samples/ && npm install
export PROJECT_ID=$DEVSHELL_PROJECT_ID
gcloud config set project $PROJECT_ID
gcloud services enable dlp.googleapis.com cloudkms.googleapis.com --project $PROJECT_ID
node inspectString.js $PROJECT_ID "My email address is jenny@somedomain.com and you can call me at 555-867-5309" > inspected-string.txt
cat inspected-string.txt
cat resources/accounts.txt
node inspectFile.js $PROJECT_ID resources/accounts.txt > inspected-file.txt
cat inspected-file.txt
gsutil cp inspected-string.txt gs://$DEVSHELL_PROJECT_ID-bucket
gsutil cp inspected-file.txt gs://$DEVSHELL_PROJECT_ID-bucket
node deidentifyWithMask.js $PROJECT_ID "My order number is F12312399. Email me at anthony@somedomain.com" > de-identify-output.txt
cat de-identify-output.txt
gsutil cp de-identify-output.txt gs://$DEVSHELL_PROJECT_ID-bucket
node redactText.js $PROJECT_ID  "Please refund the purchase to my credit card 4012888888881881" CREDIT_CARD_NUMBER > redacted-string.txt
cat redacted-string.txt
node redactImage.js $PROJECT_ID resources/test.png "" PHONE_NUMBER ./redacted-phone.png
node redactImage.js $PROJECT_ID resources/test.png "" EMAIL_ADDRESS ./redacted-email.png
gsutil cp redacted-string.txt gs://$DEVSHELL_PROJECT_ID-bucket
gsutil cp redacted-phone.png gs://$DEVSHELL_PROJECT_ID-bucket
gsutil cp redacted-email.png gs://$DEVSHELL_PROJECT_ID-bucket
```

## Troubleshooting and Solving Data Join Pitfalls

https://github.com/CloudHustlers/SEP-TRIVIA/blob/main/07_Troubleshooting%20and%20Solving%20Data%20Join%20Pitfalls%20%23GSP412%20.md


## Bracketology with Google Machine Learning
```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/2024%20Bracketology%20with%20Google%20Machine%20Learning/quicklabgsp461.sh

sudo chmod +x quicklabgsp461.sh

./quicklabgsp461.sh
```

## Troubleshooting Data Models in Looker

https://github.com/quiccklabs/Labs_solutions/blob/c0d3f96c630c98fc9ace2c68fb5f7789cf6a8102/Troubleshooting%20Data%20Models%20in%20Looker

https://www.youtube.com/watch?v=YfAaHLVQBtI

averge sales in decending order
visualization as table 
row limt =10
Top 10 Users With Highest Average Sales

## Detect and Investigate Threats with Security Command Center

https://github.com/CloudHustlers/LEVEL_2_OCT/blob/main/Detect%20and%20Investigate%20Threats%20with%20Security%20Command%20Center%20%23GSP1125%20.md

## Consuming Customer Specific Datasets from Data Sharing Partners using BigQuery

https://www.youtube.com/watch?v=ZO4Xdun30AM

https://github.com/CloudHustlers/LEVEL_1_SEP/blob/main/11_Consuming%20Customer%20Specific%20Datasets%20from%20Data%20Sharing%20Partners%20using%20BigQuery%20%23GSP1043%20.md
