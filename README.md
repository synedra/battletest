<!--- STARTEXCLUDE --->
# BattleStax 
*50 minutes, Advanced, [Start Building](https://github.com/DataStax-Examples/battlestax#prerequisites)*

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/from-referrer/)

BattleStax is a stateful JAMStack game that is wholesome fun for the entire crew.
<!--- ENDEXCLUDE --->

![image](https://raw.githubusercontent.com/DataStax-Examples/battlestax/master/tutorial/battlestax.png)


## Objectives
* Deploy a scalable JAMStack app to production
* Leverage a good CI/CD process to manage your JAMStack App
  
## How this works
The BattleStax players watch a lobby screen while playing the game on their devices.


![image](https://raw.githubusercontent.com/DataStax-Examples/battlestax/master/tutorial/architecture1.png)


[JAMstack](https://jamstack.org/) is a big leap forward in how we can write web applications that are easy to write, deploy, scale, and also maintain. Using this approach means that newly created content is rendered from a content API, while a static render of it is being built into the site for future.

## Get Started
To build and play with this app, follow the build instructions that are located here: [https://github.com/DataStax-Examples/battlestax](https://github.com/DataStax-Examples/battlestax#prerequisites)

<!--- STARTEXCLUDE --->
# Running BattleStax
Follow the instructions below to get started.

## Prerequisites
Let's do some initial setup by creating a serverless(!) database.

### DataStax Astra
1. Create a [DataStax Astra account](https://astra.datastax.com/register?utm_source=github&utm_medium=referral&utm_campaign=battlestax) if you don't already have one:
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-register-basic-auth.png)

2. On the home page. Locate the button **`Create Database`**
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-dashboard.png)

3. Locate the **`Get Started`** button to continue
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-select-plan.png)

4. Define a **database name**, **keyspace name** and select a database **region**, then click **create database**.
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-create-db.png)

5. Your Astra DB will be ready when the status will change from *`Pending`* to **`Active`** 💥💥💥 
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-db-active.png)

6. After your database is provisioned, we need to generate an Application Token for our App. Go to the `Settings` tab in the database home screen.
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-db-settings.png)

6. Select `Admin User` for the role for this Sample App and then generate the token. Download the CSV so that we can use the credentials we need later.
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-db-settings-token.png)

7. After you have your Application Token, head to the database connect screen and copy the connection information that we'll need later. We'll replace `ASTRA_DB_APPLICATION_TOKEN` with the `Token` value that is part of your Application Token.
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/astra-db-connect.png)

### Github
1. Click `Use this template` at the top of the [GitHub Repository](https://github.com/DataStax-Examples/battlestax):
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/github-use-template.png)

2. Enter a repository name and click 'Create repository from template':
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/github-create-repository.png)

3. Clone the repository:
![image](https://raw.githubusercontent.com/DataStax-Examples/sample-app-template/master/screenshots/github-clone.png)


## Running the full game
*Make sure you've completed the [prerequisites](https://github.com/DataStax-Examples/battlestax#prerequisites) before starting this step*
  - [Running on your local machine](https://github.com/DataStax-Examples/battlestax#running-on-your-local-machine)

### Running on your local machine

1. Check out the `full-game` branch
```sh
git fetch
git checkout full-game
```

2. Create a `.env` file and fill it with values from the `.env.example` file.

3. Make sure the package dependencies are installed
```sh
# install dependencies
npm install
```

3. Then, start the app in dev mode. Changes in the `src` or `functions` directories will trigger reloads.
```sh
# start battlestax in dev mode
npm run dev
```

## Tutorial Steps
The above instructions are great to get you up and running pretty quickly, but if you would like to learn how to fully deploy the application to production with JAMStack then click the button below to get started.

<p align="center">
<a href="https://github.com/DataStax-Examples/battlestax/wiki">
 <img src="https://dabuttonfactory.com/button.png?t=Open+the+workshop&f=Roboto-Bold&ts=26&tc=fff&hp=45&vp=20&c=11&bgt=unicolored&bgc=15d798" />
</a>
</p>

<!--- ENDEXCLUDE --->
