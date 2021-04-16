# COSC-310-projectgroup

The patient wants to either book an appointment or verify the appointment is booked so they open the chatbot:
There is a check to a small dataset to show its application but it can easily be used to link up to a real database of users.
Every stage of the conversation is a level:

Level 0: Registration

Level 1: Verify if meeting is booked

Level 2: Verify date

Level 3 + Are additional levels of responses 

There is a run through a level system where the user responds to questions and continues until completion. 

The GUI is there to make the bot a little nicer to use instead of just typing everything into the terminal. This makes hte bot more practical in the real world. The GUI also allows us to see what has already been said during the conversation

The bot throws the users input out to an API that then allows it to see if it is a positive response or a negative response and then responds accordingly. The API sees synonyms of the users input to then compare it to. 

There is a review at the end to see how the user liked the bot if they wish to participate.

## List of features:


#### a synonym API:
The API allows us to throw what the user puts in into something that decodes it and relates it to whether or not the response is positive or negative to the question. Without this it would be loads more coding to account for whatever the user inputs or writing every response they can put in at each point. 

![](images/ShowingAPI.png)

#### Google geocoding API:
This api takes postal addresses and converts them into latitude and longitude coordinate. This api is crucial because it provides the data that the directions API requires in order to calculate the routes.

#### Directions API
DISCLAIMER: I did not use the google directions API because I was having a lot of issues with it and several of my group members also had issues or they ran out free calls. Due to how late I started this project, I opted to use the TrueWay Directions API that is on RapidAPI.com as it didn't give me as much trouble parsing out the data from the JSON file. I know we were required to gain approval before using a non-listed API but I didn't have enough time. I hope I don't lose my marks for this api, i worked really hard on it :)

Anyways, this API provides driving instructions to our medical clinic. It takes the geocoded address from the geocoding API and then outputs the steps to get to the destination from the provided address. 

#### GUI:
This allows the user to see the inputs that they already put in in a box display. Including this makes the bot more easily understood. Being able to see what was already put in without the use of the console allows the user an informed decision if they forgot what was asked before. (see above image for GUI)

#### review process(not on official list):
Though not formally on the assignment features this would in theory help us gather what parts of the bot are working or not for the users. With feedback we could then sift through it and figure out what works best and what doesnt work. 

![](images/midReview.png)


#### spell checking inputs:
This is included with the API. Now if the user accidentally adds a character they did not want the bot will still recognize the response. 

![](images/spellCheck.png)

    
