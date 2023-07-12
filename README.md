# Introduction 
This project runs a basic service for a chatgpt bot on discord. The configuration includes three parties. 
1. Discord. One needs to create a chatbot on discord, configure the appropriate authorities and 0auth2 info, and add the chatbot to a discord service. Once suceed, one shall see a message like "<YOUR-CHATGPT-BOT> has joined the channel" on your discord service. 
2. OpenAI. One needs to have the openai api key. Note that subscription of api service is different from subscription of chatgpt service. To control cost, one shall set up the hard and soft limits. If one doesn't have an open api key, then he can generate one and MUST note it somewhere safe as one can no longer see it after its geenralisation. Keep the api key safe, which means not exposing it to browser or other cliend-side code. If in risk of leak, discard and generate a new one. 
3. Node.js project. The openai api key and discord chatbot token are stored in `.env` and should not be exposed. 

For better experience, one might consider running the node.js service on an aws server for persistent service. 

# How to start the service
1. Run `node index.js` to start the service
2. Now talk with the chatbot in the discord service 

