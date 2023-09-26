# nosql_mini_project_1

# Chatchat Chatbot

## Table of Contents
- [Introduction](#introduction)
- [Commands & Functionality](#commands--functionality)
- [Instructions](#instructions)

## Introduction
The Chatchat Chatbot is a Python-based redis (uses Redis for data storage) chatbot project. The Chatchat has multiple features like weather, fun facts, identify users, channel communications. Thank you for any questions, feedbacks and suggestions. I am more than happy to add other functionalities you like!

## Commands & Functionality

### General Commands
- !help: Displays a list of all available commands and their usage.
- !weather <city>: Provides the current weather conditions for the specified city.
- !fact: Delivers a random fun fact.
- !whoami: Displays stored user information.
- !exit: Exit the chatbot

### Channel Commands
- identify: Identify yourself to the chatbot.
- join <channel>: Join a specified channel to send and receive messages.
- leave <channel>: Leave a channel you previously joined.
- send <channel> <message>: Send a message to all users in a specified channel.

#### Extra Credit Commands:
- send to [user] [message]: Send a private message to a specific user
- change to [color]: Change the color of your messages

## Instructions

### Packages & Environment
- Docker
- Python
- Redis

### Setup
- Run `docker-compose up` to activate python and redis containers (Allow these two containers to connect)
- Run `docker exec -it <container_id> bash` to go to python container
- Run `docker exec -it <container_id> redis_cli` to redis_cli container
- Run `python mp1_template.py` to start


#### Use Chatbot
1. You will be asked to enter some basic information; the information will then be stored, so next time you enter the chatbot, you will only be asked to enter username if there is an existing username

2. You can then play around the general commands

3. You can also play around with the channel commands and monitor the activities in channels by running `MONITOR` in redis-cli:
![114711695703851_ pic](https://github.com/ellerywuyn/nosql_mini_project_1/assets/47910316/79154384-5e83-4be6-9ab4-5315bbc0b9ed)

4. You can also use the QA functionality if you have any question to GPT4

## GenAI Usage
I used ChatGPT to help me generate a list of fun facts.
