# PHPWebsite
A website for my final project of CS 234 Databases and Web Development. It includes a login screen, home page with video game characters, a secondary page with game recommendations, another page which allows users to give a game review or game recommendation, and an admin page with CRUD functions.

LOGIN SCREEN ---
To log in, you must be a registered user otherwise it gives an error. Below the 'Login' buttion, there is a 'Register' button. This allows users to register into my database and are granted access to login into my page. The username must be unique and the password must be 7-15 characters and contain a number or else the user will be given an error.

HOME PAGE ---
This page is very simple, it is just a list of 4 video game characters. It is just a joke as it is the same character using different aliases, but a list nonetheless. On the top left corner, you are given three options: go to a site with recommended games, go to a site which allows you to leave a game review or game recommendation, or logout (this kills the users session and takes them out of the site).

REVIEW/RECOMMENDATION ---
The review or recommendation lets the user use one of these options. They are both linked to a respective one-to-many sql table which is linked to the registered_table (all registered usernames and passwords). From there, it takes the reviewing user's username and saves it with their review and/or recommendation along with a unique numerical id. Both of these tables are set to cascade with its parent table so that when the admin powers are used, they are also updated or deleted in these two tables as well.

ADMIN PAGE ---
This admin page gives the admin access to see all registered users. The admin can also add new users, however the username must be unique or else you are given an error. The admin can update usernames and delete users as well. In order to access this admin page, I made a separate admin login page in which you must use the hard-coded admin username and password to access the page, if you use the wrong username/password you are given an error and denies access.

DISCLAIMER ---
In order to use this, you must have MAMP servers on as well as php downloaded and functioning properly.
