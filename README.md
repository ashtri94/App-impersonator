# App-impersonator
Think about your favorite apps, and pick one that stores your data- like a game that stores scores, an app that lets you post updates, etc. Now in this project, you're going to imagine that the app stores your data in a SQL database (which is pretty likely!), and write SQL statements that might look like their own SQL.  CREATE a table to store the data. INSERT a few example rows in the table. Use an UPDATE to emulate what happens when you edit data in the app. Use a DELETE to emulate what happens when you delete data in the app.
CREATE TABLE money_manager (
id INTEGER PRIMARY KEY AUTOINCREMENT,
Date INTEGER,
payment_type TEXT,
Category TEXT,
Amount INTEGER);

INSERT INTO money_manager (Date,payment_type,Category,Amount)
VALUES ("01/06/2021","sbi account","gogrocio",3957);
INSERT INTO money_manager (Date,payment_type,Category,Amount)
VALUES ("02/06/2021","sbi account","S2 bazaar",185);
INSERT INTO money_manager (Date,payment_type,Category,Amount)
VALUES ("03/06/2021","sbi debit card","electricity bill",1336);
INSERT INTO money_manager (Date,payment_type,Category,Amount)
VALUES ("04/06/2021","sbi account","Room Rent",3000);
INSERT INTO money_manager (Date,payment_type,Category,Amount)
VALUES ("05/06/2021","cash","S2 bazaar",60);
INSERT INTO money_manager (Date,payment_type,Category,Amount)
VALUES ("06/06/2021","sbi debit card","amazon",938);

SELECT * FROM money_manager;

UPDATE money_manager SET payment_type = 'sbi account' WHERE id = 5;

SELECT * FROM money_manager;
