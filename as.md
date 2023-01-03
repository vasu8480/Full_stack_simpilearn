#Create a document called Assignment for MongoDB
Create a collection/Table called Customer having the following fields:
• customerid
• customername
• address
• customertype
• status
• value in customer type is
• gold
• silver
• guest

db.customers.insertMany([  { "customerid": C00013, "customername": "Alice", "address": "123 Main St", "customertype": "gold", "status": "active" },  { "customerid": 2, "customername": "Bob", "address": "456 Maple Ave", "customertype": "silver", "status": "active" },  { "customerid": 3, "customername": "Charlie", "address": "789 Oak St", "customertype": "guest", "status": "active" }])
