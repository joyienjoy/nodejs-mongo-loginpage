STEP BY STEP PROCESS:

INSTALL NODEJS:

curl -fsSL https://deb.nodesource.com/setup_19.x | sudo -E bash - && sudo apt-get install -y nodejs

INSTALL MONGODB

wget -qO - https://www.mongodb.org/static/pgp/server-6.0.asc | sudo apt-key add -

echo "deb [ arch=amd64,arm64 ] https://repo.mongodb.org/apt/ubuntu focal/mongodb-org/6.0 multiverse" | sudo tee /etc/apt/sources.list.d/mongodb-org-6.0.list

sudo apt-get install -y mongodb-org

sudo systemctl start mongod

sudo systemctl status mongod

------------------------------
mongosh

>> use ManualAuth   ## whatever database name you want as present in server.js
>> createUser   

-----------------------------
execute program: npm start
