laman-language


http:(half duplex)
google.com----req--->server
google.com<----res---server
then tcp connection is closed after getting the response
google.com----req--->server
google.com<----res---server
then tcp connection is closed after getting the response

it is the unidirectional stateless protocol( this lead to send req to get response everytime)

-----to overcome this -----
we have polling
-long polling
-short polling
in this we set a interval to send the request at particular interval of time in timely manner we send req and wait for response
drawback like in messageing if other user doesnot send anyb message but send the req and in respoins eit get a n empty reponse it lead wastage of resource

----to overcome this-----

sever sent events their is a unidirectional trasfer from the server;
like broadcasting,insta feeds

---- chatgpt is using sse----

----------WEBSOCKET--------(it is bi-directional statefull and full duplex)

keep in mind that our 1st req for the websocket is http request to established a connection

now client server we can send data through server <---> client
