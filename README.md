# Moduit
Moduit Challange

Following are the steps to run a monitor API in Postman:

1. Login to Postman account at https://app.postman.com/
2. Click on the "Monitor" menu on the left sidebar.
3. Select "Moduit" monitor. Once the monitor is selected, you will be redirected to the "Monitor Details" page. On this page, you can see the status of the monitor and the last activity history of the monitor.
4. If you want to start the monitor, click the "Start" button on the "Monitor Details" page.
The monitor will start running according to the preset settings.

NOTE :
The reason why I chose the following 4 APIs from reqres (CREATE USER -> UPDATE USER -> DELETE USER -> LIST USERS)

Because when creating a user, the user that is created is not stored in the reqres DB (you can check with the hit api list user which will display a user that's just that or a static user), that's why when I CREATE USER -> GET SINGLE USER (the user that has been created is not in this response, because the id is considered not found. because the data created is not stored in the DB reqres. then I trick it with a hit api UPDATE USER using the id obtained from the api CREATE USER -> after that do DELETE with the same id and finally hit api LIST USERS (because it is static).