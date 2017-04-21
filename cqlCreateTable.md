CREATE KEYSPACE testTweets WITH replication = {'class': 'SimpleStrategy', 'replication_factor': 3} AND DURABLE_WRITES=true;
use testTweets;
CREATE TABLE tweets(id uuid PRIMARY KEY, created_at text , date text, status text, hashtags set<text>);
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-47ff-b370-5ddebb2de429,'2:00','4202017',{'Dylan','Elliot'}, 'Big Data is fun');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-45ff-b370-5ddebb2de429,'3:00','4202017',{'Dylan'}, 'Big Data is not fun');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-47ff-c370-5ddebb2de429,'4:00','4202017',{'Evan','Peter'}, 'The Green Gopher strikes again!');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f787-46ff-b370-5ddebb2de429,'5:00','4202017',{'Evan','Elliot'}, 'Class is lit');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-47ff-b370-5ddebb2de429,'6:00','4202017',{'Dylan'}, 'Mumford and Sons rock');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-47ff-b372-5ddebb2de429,'7:00','4202017',{'Peter','Elliot'}, 'Karate is fun');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-47ff-c370-5ddebb2de429,'8:00','4202017',{'Evan','Peter','Dylan','Elliot'}, 'The tap is not open');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-41ff-b370-5ddebb2de429,'9:00','4202017',{'Peter','Dylan'}, 'We got beer');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-42ff-b370-5dhebb2de429,'8:00','4202017',{'Evan', 'Elliot'}, 'Pearl is empty');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-48ff-b370-5djebb2de429,'10:00','4202017',{'Peter','Dylan','Elliot'}, 'Pearl is not empty');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-47df-b370-5deebb2de429,'13:00','4202017',{'Peter','Dylan','Elliot'}, 'Evan is not in this tweet');
INSERT INTO tweets (id, created_at, date, hashtags, status) VALUES (4214783a-f687-47af-b370-5ddebb2de429,'15:00','4202017',{'Dylan','Elliot'}, 'trash can is on fire');