# rock_paper_scissors_demo

1. initialize the project in the current directory with cmd: rasa init
2. if you get error saying rasa cmd not found -> if we are using linux, recheck that we should activate the virtual environment.
3. cmd to activate the virtual environment -> go to the folder where venv folder is present and type the cmd: source ./venv/bin/activate
4. once the application is initialized and we have basic structure to start with, we will continue with our development
5. First of, we will start with domain file where we will specify all are intents, entities that we get as input from the users, slots which are used for storing inputs from users, responses that assistant says, and actions which will run particular actions files based on the user input
6. once we have made changes in domain.yml file, we will update the nlu.yml file
7. nlu.yml file is to specify some examples to particular intents
8. And then, we will update our stories.yml file. We need to write stories in such a way that our users are expected to interact with the bot and the bot has to respond respectively
9. Remember intents are user driven while actions are for bots
10. In domian.yml file we will mention actions which represents our logic present in actions/actions.py file
11. Once we have written the logic, it is time to train and run the application
12. After making changes we need train. cmd for that is: rasa train
13. once you enter the command, there will be a model generated under models folder.
14. we then have to run our actions file. Before that, make sure you have uncommitted/update the action_endppoint for our actions in endpoint.yml file
15. rasa run actions is the command to run the actions
16. At this point we have our model trained and actions running
17. open a terminal to play the rasa cli chatbot
18. Type rasa shell in new terminal to enter rasa cli. Finally we can play with the chatbot
