# MongoDB Atlas sample data dump and restore

## Dump from Atlas:
mongodump --uri mongodb+srv://username:password@sandbox.abc12.mongodb.net/sample_training<br>
where:<br>
- cluster name: sandbox
- database name: sample_training


## Start mongod.exe on localhost
if not exist "c:\data\" mkdir "c:\data"<br>
if not exist "c:\data\db" mkdir "c:\data\db"<br>
"c:\Program Files\MongoDB\Server\5.0\bin\mongod.exe" --dbpath="c:\data\db"<br>

## Local restore
mongorestore --drop --db sample_training sample_training/