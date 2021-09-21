
# Lab 3 - MongoDB

## Getting started
- Getting started was done as descibed, even though the bulletpoints in the assignment used different words to describe the 5 of the 6 tabs on the webiste at this current date. The assignment is probably written for a previous iteration of the same tutorial.


## Installation 
- The installation was done according to [this tutorial](https://docs.microsoft.com/en-us/windows/wsl/tutorials/wsl-database#install-mongodb). Verifying the package is done by the package manager, via the apt install command. 


## Experiment 1

Only 2 or fewer screenshots are given per CRUD operation  

### Inserting

![img.png](images/img.png)
![img_1.png](images/img_1.png)

### Query
![img_4.png](images/img_4.png)
![img_5.png](images/img_5.png)

### Update
![img_6.png](images/img_6.png)
![img_7.png](images/img_7.png)

### Remove

The items added to the collection and deleted:
![img_9.png](images/img_9.png)

Delete all that have status A:
![img_10.png](images/img_10.png)

### Bulk write
It is almost the same as the 2. image in [Write](/dat250-expass3.md#Write) section 
![img_11.png](images/img_11.png)

## Experiment 2

MapReduce's method is deprecated so aggregation pipeline was used instead.

Example from the tutorial:
![img_13.png](images/img_13.png)

The self developed pipeline aggregation operation:

```MongoDB
db.orders.aggregate([
{ $match: {ord_date: {$lt:ISODate("2020-03-23T00:00:00.000Z")}}},
{ $group: { _id: "$cust_id", value: { $sum: "$price" } } },
])
```

The idea was to filter orders that were made before the specified date.
![img_12.png](images/img_12.png)
As one can see, Don Quis order total was the one who had his sum reduced from 155 to 130, meaning that Don Quis had an order after the specified date. 
