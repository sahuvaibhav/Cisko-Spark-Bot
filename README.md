# Python ChatBot Basic Script for demo to Intergrate with Cisco Spark

### References : 
https://github.com/SamPiy93/Python-Bot-Integration

http://madumal.piyasundara.org/2017/02/python-chat-bot-integration-with-cisco.html

Below are some basic steps involved
# How to set a webhook for Cisco Spark
1. Use ngrok for making localhost:port to public safely (Install ngrok free )
2. use command 'ngrok http <port>'
3. Now Register a webhook at cisco spark using https://developer.ciscospark.com/endpoint-webhooks-post.html# in this link use 
     - authorization: Bot access token
     - targetUrl: <ngrok link>/
     - resource: messages
     - event : create
     - filter: roomId=room_id (as below)
This will register ngrok link to webhook 
5. Now run this file using python starterbotCiscoSpark.py

# Supporting links 
1 - http://madumal.piyasundara.org/2017/02/python-chat-bot-integration-with-cisco.html

2 - https://communities.cisco.com/community/developer/spark/blog/2016/07/18/spark-bot-demo

3 - https://developer.ciscospark.com/endpoint-rooms-get.html to get room ids

4 - https://developer.ciscospark.com  to create a new bot 

5 - https://learninglabs.cisco.com/lab/collab-spark-chatops-bot-itp/step/1  Lab for many bots ay cisco spark

6 - https://learninglabs.cisco.com/lab/collab-sparkwebhook/step/1  webhook understanding good one
  
## For detailed explaination follow my Blog at meduim 
 https://medium.com/@vaibhavsahu/how-to-integrate-your-chatbot-with-cisco-spark-c6b8188c6948
 
## Summary


