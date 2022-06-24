# MongoDb Quick Ref

  * NoSql, Non Relational Database
  * Store JSon
  * Easy to get started
  * Free cloud hosting--Atlas

### what is a Database?

    In MongoDB, a database can be defined as a physical container for collections of data. Here, on the file system, every database has its collection of files residing. Usually, a MongoDB server contains numerous databases.

### RDBMS MongoDb Difference

Here is a table showing the relation between the terminologies used in RDBMS and MongoDB:


    RDBMS	            MongoDB

Database	            Database
Table	                Collection
Tuple or Rows	        Document
Column	                Field
Table Join	            Embedded Documents
Primary Key	            Primary key / Default key
Mysqld / Oracle	mongod


* MongoDb is a JSON(javascriptObjectNotation) Format

* Mongodb stores doucment in BSON(Binary JSON)

## JSON vs BSON Diff...

JSON is support 6 data Type

* String
* Number
* Boolean
* Array
* Object
* Null


BSON is Support data type

* Strig
* Double
* 32-bit integer
* 64-,,
* Boolean
* Array
* object
* Null
* Regular Expression
* Timestamp
* Binary Data
* Date
* Objectid  --> this is primery key
and others


# How to work mongoDB

  server
  client to the mongoDB is working

# How to start server

* open terminal-->mongod and the start the server
* open another terminal-->mongo type is a Client

# WHo is using MongoDB...?

* facebook,Google,EA,Sega,ebay


### Basic Commands on Mongo Shell

1. show active database --> (db)
2. List all available databae --> (show dbs)
3. change Active database --> (use dbname)
4. Create Database  --> (use dbname new value sent to the database new created )
5. Create new Collecion -->(db(dbname).createCollection("user"))
6. Delete Collection -->(db.getCollection("collection name").drop())
7. Delete Collection -->(db.dropDatabase())
8. Help --> db.help()

### Insert new Doucment
1. Insert -->db.collectionname.insert({name:"selva"})
2. InsertOne -->insert & insertOne is same new version
3. InsertMany --> db.collectionname.insertMany([{},{}])

### Read Doucment
1. Find Doucment --> db.collectionname.find()
2. Find One Doucment --> db.collectionname.findOne()