# thecardboard

## Requirements
You need to setup docker and visual studio code.  This article helped me get my environment configured

https://medium.com/@jasonterando/debugging-with-visual-studio-code-xdebug-and-docker-on-windows-b63a10b0dec
## About the cardboard
There are 4 accounts: admin, moderator, user1, and user2.  All passwords are "cardboard".

Any changes that need to be preserved in the database should be commited by running the following command on the mysql container:

`mysqldump -p cardbd_mybb > /docker-entrypoint-initdb.d/data.sql`
