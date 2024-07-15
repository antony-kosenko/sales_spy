# Sales Spy
Microservise project consists of 3 applications which together form complete service for :
1. **Requesting**. Serivice interacts with user in some convinient method such a chat-bot or web UI to get requested item url(s) on particular e-commerce store (which evailable for monitoring);
2. **Recording**. Backend recieves requests from *requesting* service and stores user's request data which basicaly consist of user identifications and items' url(s) requested;
3. **Parsing**. Parses an requested urls store in backend and makes some processing of results. If result has a positive progression e.g. price drop relative to base price then notifies a *recording* service which passes relative data to an user through *requesting* service to an user using notification messages.
