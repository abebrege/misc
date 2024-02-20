# Setup Guide to Write Swagger Documentation

## Links needed
1. http://localhost:8084/swagger/#/
2. http://localhost:8085/login 
3. https://www.postman.com/downloads/


## Postman Setup
1. Navigate to [link 3](https://www.postman.com/downloads/)


2. Download and setup your Postman account
3. Start your local frontend and backend 
4. Navigate to [link 2](http://localhost:8085/login)
5. Before logging in, press `Ctrl + Shft + i` to open up development tools
6. Login using the appropriate user credentials (most likely admin@northcrossgroup.com)
7. Navigate to the **Application** tab in dev tools, in the **Storage** tab, expand the **Session Storage** section, and click on **http://localhost:8085**
8. Copy the **accessToken** value ("eyJhbGc...bZQ15YwyJe0")
9. In Postman, click on the **Headers** tab.
10. In the **key** section enter `x-access-token` and in the **value** section enter in the **accessToken** you copied from login. Be sure to delete the quotes at the begging and end of the key

## Using Postman
1. In your backend application folder in VS, navigate to **app>swagger** and pick a .yml file. In this case I will use **(boardMemo.yml)**


2. Navigate to **app>routes**, and select the route that correlates to the .yml file chosen. **(boardMemo.routes.js)**
3. At the bottom of the **boardMemo.routes.js** you will find a block of code that reads ```app.use("/api/boardMemo", router);```
Copy the **"/api/xxx"** portion. 
4. In Postman, to the right of the green **GET** in the text box, enter **localhost:8084** folloed by the **/api/xxx** that you just copied. (Results should look as so: **localhost:8084/api/boardMemo/**)
5. Navigate to [link 1](http://localhost:8084/swagger/#/)
6. Find your route **(BoardMemo)** and select a **GET** route. Copy the path to the right of **GET** (in this case it is `/boardMemo/application/{applicationId}`)
7. To get the application ID, scroll and find the example ID given. In this case it is `4a10da5e-54f0-4dbd-b137-8da3534c7e7c`
8. Open Postman and add the two items to the end of your URL. Your URL in the textbox shoud now read ``