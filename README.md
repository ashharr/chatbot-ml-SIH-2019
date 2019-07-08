# chatbot-ml-SIH-2019
A Customer Support Chatbot using Machine Learning for Smart India Hackathon 2019 ( Winning Idea)

Problem Definition / Idea:

The Solution is that we have created a chatbot that responds to the request made by the customer by searching the DB for solutions. 
Our chatbot is capable enough to interpret to all queries of the customers , analyze them and understand the intent of the queries. 
The chatbot shall search the entire database for resolution to the problems. If the best solution is found then Chatbot will directly 
provide the solution to the customer's concerned queries. On the contrary , if no solution is found, then chatbot will handover the
problem to the Support Staff available to interpret the query and provide a better solution by interacting with the customer. Having
interacted with the customer and finding new solutions for different queries, the solutions would get updated in the data base wherein
the chatbot shall be prepared to handle similar queries in future.
The Database has been maintained using SQL Alchemy and will be integrated with the NLP engine using Dialogflow API’s which can accomplish word embedding
intent and entity detection.




Technology Stack:

1. Dialogflow(NLP training and Webhook):

	Dialogflow which is powered by Google was used to create intents and entities with respect to the domain that was selected i.e.
  Mutual Funds. 

Based on the intents the Chatbot was trained, Small Talk is a feature offered by Dialogflow was also incorporated into the Chatbot. 

2.  Python ( Sentimental Analysis and Sentence similarity )

	To work on the default fallback intent we used python modules such as vaderSentiment to do Sentimental analysis so as to verify
  whether the query is a Feedback or a Complaint. Part of speech tagging was also done using NLTK.corpus module.

3. Flask(API and REST API)

      Representational State transfer (REST)  API was used as a web API and was implemented using flask microframework.

4. SQLAlchemy(Data Base)

      The identified query which is fallback content is updated in the database to provide its solution when asked the next time

5. Ngrok(local web server)

Secure web tunnel was created to handle the requests along with public URL. It listens on the same port that your local web server is running on.

This URL was used to connect to Dialogflow API using webhook feature.


Integrations:

Whatsapp using Twilio

Skype

Telegram

Google Assistant
