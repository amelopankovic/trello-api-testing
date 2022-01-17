# Trello-api-testing

## Project description

In this project I have created smoke test for Trello - Task Management App. Test is fully automated and it can be used for checking the main functionality of the app. I have used Postman API Platform for creating tests and Trello REST API documentacion for API calls.
 

### Running tests with Postman

Import Trello_collection.json and Trello_environment.json files into the Postman aplication. 
Pass in your Trello API key and token in collection variables under "oauth" variable, also create another Trello account and enter API key and token for that account under "oauthNewMember" variable. Generate your [API key and token](https://trello.com/app-key).
Click on the Runner button and drag the Collection to Run Order window. Click on the "Run Trello" button. 

### Running tests with Newman

Export collection and environment files from postman and replace them in trello-api-testing folder. 
This is necessary because you have entered your keys and tokens for authorization.

If you have npm installed, run this command in your command-line interface (CLI) `npm install -g newman`.

After installing Newman, navigate to trello-api-testing folder in CLI and run smoke test: `newman run Trello_collection.json -e Trello_environment.json`.
