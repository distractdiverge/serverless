# Hello World Serverless App
This is a quick and simple NodeJS app written for the serverless platform.
This can be deployed on Google Cloud, Azure, or AWS.

*Note: I use ```yarn``` here, but the project is setup to use ```npm``` as well.* 

## Getting Started
1. Clone this Repo
   ```$bash
   git clone git@github.com:alexlapinski/serverless.git
   ```
2. Login to *Serverless*
   ```$bash
    yarn run sls login
   ```
3. [Setup AWS <-> Serverless (if not already done)](https://github.com/serverless/platform/blob/master/docs/setup-aws-account.md)
4. Setup Serverless with AWS Credentials

    **Option 1** - Serverless Config Command
    ```bash
    yarn run sls config credentials --provider aws --profile serverless --key <AccessKey> --secret <SecretKey>
    ```
     
    **Option 2** - Update the ```~/.aws/credentials~``` file, using 'serverless' as the profile name
    
    *Note: You can use any profile name, just make sure the ```serverless.yaml``` file is updated*