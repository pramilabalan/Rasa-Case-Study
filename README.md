# Rasa-Case-Study
The goal of this case study is to build a conversational bot (chatbot) which can help users discover restaurants across several Indian cities. 


The main purpose of the bot is to help users discover restaurants quickly and efficiently and to provide a good restaurant discovery experience. The project brief provided to you is as follows.
 

The bot takes the following inputs from the user:

**City**: Take the input from the customer as a text field. For example:

  Bot: In which city are you looking for restaurants?

  User: anywhere in Delhi

**Cuisine Preference**: Take the cuisine preference from the customer. The bot should list out the following six cuisine categories (Chinese, Mexican, Italian, American, South Indian & North Indian) and the customer can select any one out of that. Following is an example of the same:

  Bot: What kind of cuisine would you prefer?

  Chinese
  Mexican
  Italian
  American
  South Indian
  North Indian
  
  User: I’ll prefer Italian!
  
**Average budget for two people:** Segment the price range (average budget for two people) into three price categories: lesser than 300, 300 to 700 and more than 700. The bot should ask the user to select one of the three price categories. For example:

  Bot: What price range are you looking at?

  Lesser than Rs. 300
  Rs. 300 to 700
  More than 700
  User: in range of 300 to 700
  
  
  
While showing the results to the user, the bot should display the top 5 restaurants in a sorted order (descending) of the average Zomato user rating (on a scale of 1-5, 5 being the highest). The format should be: {restaurant_name} in {restaurant_address} has been rated {rating}.


Finally, the bot should ask the user whether he/she wants the details of the top 10 restaurants on email. If the user replies 'yes', the bot should ask for user’s email id and then send it over email. Else, just reply with a 'goodbye' message. The mail should have the following details for each restaurant:

  Restaurant Name
  Restaurant locality address
  Average budget for two people
  Zomato user rating


Accomplished the following in the project:

**NLU training**: Used rasa-nlu-trainer to create more training examples for entities and intents. 

**Built actions for the bot:** Read through the Zomato API documentation to extract the features such as the average price for two people and restaurant’s user rating. Built an ‘action’ for sending emails from Python.

**Created more stories**: Used train_online.py file to create more stories. 
