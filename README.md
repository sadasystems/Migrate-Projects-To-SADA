# Migrate to SADA Billing Account 
Migrate your projects that are currently connected to your legacy billing account to SADA billing account 

## Getting Started
Make sure node and gcloud is installed on your system

gcloud - [https://cloud.google.com/sdk/docs/install](https://cloud.google.com/sdk/docs/install)

nodejs - [https://nodejs.org/en/download/](https://nodejs.org/en/download/)

## WARNING: USER NEEDS BILLING ACCOUNT ADMINISTRATOR ROLE FOR YOUR SADA BILLING ACCOUNT 

#### 1. Clone the repository and navigate to the directory
```shell
git clone https://github.com/sadasystems/Migrate-Projects-To-SADA.git 
cd Migrate-Projects-To-SADA
```
#### 2. Authenticate yourself with Google
Install gcloud beta
Make sure this user has sufficient permissions at YOUR ORGANIZATION level IAM
```shell
gcloud components install beta --quiet
gcloud default application login 
gcloud init
```

#### 3. Install all dependencies with clean install
```shell
npm install
```

#### 4. Run Script
```shell
In the .env file, add old billing account ID and sada billing account ID
```

#### 5. Run Script
```shell
node main.js
```

### It will take 1-2 minutes to process through all the projects (be a little patient! :))
