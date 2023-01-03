#Create a document called Assignment for MongoDB
  db.createCollection("customers", {
  "customerid": 1,
  "customername": 1,
  "address": 1,
  "customertype": 1,
  "status": 1
})



db.customers.insertMany([
  { "customerid": "C00013", "customername": "Holmes", "address": "London", "customertype": "gold", "status": "active" },
  { "customerid": "C00001", "customername": "Micheal", "address": "New York", "customertype": "guest", "status": "inactive" },
  { "customerid": "C00020", "customername": "Albert", "address": "New York", "customertype": "silver", "status": null },
  { "customerid": "C00025", "customername": "Ravindran", "address": "Bangalore", "customertype": "gold", "status": "inactive" },
  { "customerid": "C00024", "customername": "Cook", "address": "London", "customertype": null, "status": null },
  { "customerid": "C00015", "customername": "Stuart", "address": "London", "customertype": "gold", "status": "active" },
  { "customerid": "C00002", "customername": "Bolt", "address": "New York", "customertype": "gold", "status": "active" },
  { "customerid": "C00018", "customername": "Fleming", "address": "Brisban", "customertype": "silver", "status": "inactive" },
  { "customerid": "C00021", "customername": "Jacks", "address": "Brisban", "customertype": "guest", "status": "active" },
  { "customerid": "C00019", "customername": "Yearannaidu", "address": "Chennai", "customertype": "guest", "status": "active" },
  { "customerid": "C00005", "customername": "Sasikant", "address": "Mumbai", "customertype": "gold", "status": "inactive" },
  { "customerid": "C00007", "customername": "Ramanathan", "address": "Chennai", "customertype": "silver", "status": "inactive" },
  { "customerid": "C00022", "customername": "Avinash", "address": "Mumbai", "customertype": null, "status": null },
  { "customerid": "C00004", "customername": "Winston", "address": "Brisban", "customertype": "gold", "status": "active" }
])

1.find all the customers
  -db.customers.find()

2.find the count of customer
  -db.customers.find().count()

3.display the first customer
  -db.customers.find().limit(1)

4.display first 5 customers
  -db.customers.find().limit(5)

5.find the active customers
  -db.customers.find({status:"active"})

6.find the inactive customers
  -db.customers.find({status:"inactive"})

7.find the customers who are gold
  -db.customers.find({customertype:"gold"}) 

8.find the customers who are silver
  -db.customers.find({customertype:"silver"})

9.find the customers who are gold and active
  -db.customers.find({customertype:"gold",status:"active"})

10. find the customer who has customer type as null and status null
  -db.customers.find({customertype:null,status:null})

11.find the customer who has customer type as not null
  -db.customers.find({customertype:{$ne:null}})

12.find the customer who lives in Mumbai ,Chennai and Bangalore
  -db.customers.find({address:{$in:["Mumbai","Chennai","Bangalore"]}})

13. find the customer who lives in Brisban
  -db.customers.find({address:"Brisban"})

14. find the customer who lives in other than newyork and london
  -db.customers.find({address:{$nin:["New York","London"]}})

15. update customer , set customertype='premium' for those staying in London
  -db.customers.updateMany({address:"London"},{$set:{customertype:"premium"}})

16. update customer set customertype='Gold' whose value is null
  -db.customers.updateMany({customertype:null},{$set:{customertype:"Gold"}})

17. update customer set status='Active' whose value is null
  -db.customers.updateMany({status:null},{$set:{status:"Active"}})

18. create an index on address so that search will be faster
  -db.customers.createIndex({address:1})

19. delete customer cook, bolt and winston
  -db.customers.deleteMany({customername:{$in:["Cook","Bolt","Winston"]}})




#PostgreSQL
CREATE TABLE customer (
  customerid TEXT NOT NULL PRIMARY KEY,
  customername TEXT,
  address TEXT,
  customertype TEXT,
  status TEXT 
);
INSERT INTO customer (customerid, customername, address, customertype, status)
VALUES 
('C00013', 'Holmes', 'London','gold','active'),
('C00001', 'Micheal', 'New York','guest','inactive'),
('C00020', 'Albert', 'New York', 'silver',null),
('C00025', 'Ravindran', 'Bangalore', 'gold','inactive'),
('C00024', 'Cook', 'London', null,null),
('C00015', 'Stuart', 'London', 'gold','active'),
('C00002', 'Bolt', 'New York', 'gold','active'),
('C00018', 'Fleming', 'Brisban', 'silver','inactive'),
('C00021', 'Jacks', 'Brisban','guest','active'),
('C00019', 'Yearannaidu', 'Chennai', 'guest','active'),
('C00005', 'Sasikant', 'Mumbai', 'gold','inactive'),
('C00007', 'Ramanathan', 'Chennai','silver','inactive'),
('C00022', 'Avinash', 'Mumbai',null,null),
('C00004', 'Winston', 'Brisban','gold','active');

1. find all the customers
  -SELECT * FROM customer;

2. find the count of customer
  -SELECT COUNT(*) FROM customer;

3. display the first customer
  -SELECT * FROM customer LIMIT 1;

4. display first 5 customers
  -SELECT * FROM customer LIMIT 5;

5. find the active customers
  -SELECT * FROM customer WHERE status='active';

6. find the inactive customers
  -SELECT * FROM customer WHERE status='inactive';

7. find the customers who are gold
  -SELECT * FROM customer WHERE customertype='gold';

8. find the customers who are silver  
  -SELECT * FROM customer WHERE customertype='silver';

9. find the customers who are gold and active
  -SELECT * FROM customer WHERE customertype='gold' AND status='active';

10. find the customer who has customer type as null and status null
  -SELECT * FROM customer WHERE customertype IS NULL AND status IS NULL;

11. find the customer who has customer type as not null 
  -SELECT * FROM customer WHERE customertype IS NOT NULL; 

12. find the customer who lives in Mumbai ,Chennai and Bangalore
  -SELECT * FROM customer WHERE address IN ('Mumbai','Chennai','Bangalore');

13. find the customer who lives in Brisban
  -SELECT * FROM customer WHERE address='Brisban';

14. find the customer who lives in other than newyork and london
  -SELECT * FROM customer WHERE address NOT IN ('New York','London');

15. update customer , set customertype='premium' for those staying in London
  -UPDATE customer SET customertype='premium' WHERE address='London'; 

16. update customer set customertype='Gold' whose value is null 
  -UPDATE customer SET customertype='Gold' WHERE customertype IS NULL;

17. update customer set status='Active' whose value is null
  -UPDATE customer SET status='Active' WHERE status IS NULL;

18. create an index on address so that search will be faster 
  -CREATE INDEX address_index ON customer (address);

19. delete customer cook, bolt and winston
  -DELETE FROM customer WHERE customername IN ('Cook','Bolt','Winston');



