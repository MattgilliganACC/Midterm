Consider the following snippet of MongoDB query code.  Please explain what is happening.

    `db.mycol.find({},{"title":1,_id:0}).limit(2)`

### Solution here please ...

It is querying the database, but only returning 2 documents rather than the entire contents. 
