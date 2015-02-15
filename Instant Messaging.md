#Instant Messaging Desktop Application

###Idea author: Hayden Quinn

###Required Technologies
C/C++, SQL, Java/C#

###Project Description
One proposition which will allow people from different disciplines to contribute to a project is to make an Instant Messaging application. The general idea is to allow users to connect to a server, have some authentification as to who they are, be able to message an individual who they have as "friends" or a group, and be able to send small files to other users.  

The server side of this project would be coded in either C or C++ using a Network Library (e.g. Boost::ASIO) or doing it in Raw Sockets (BSD, WinSock). The server side of the application should handle users connecting to the server, process requests from users (i.e. sending a message to another user), logging user requests (i.e. storing messages from users so they can continue to chat where they left off at a later date), etc. More on server side can be brainstormed if this project gets off.

The client side of this project would be coded in either Java or C# (or any other language that you like (Java seems like a good option due to it being easier to port)). The client should be able to securely connect to the program, be able to add/delete users to their "friend's list", chat to people/groups securely, send files to peers, etc.

This is a vague description, and it is somewhat simple to build a basic IM application with Socket Programming, but to make a robust and highly distributable one could prove to be a good challenge.
