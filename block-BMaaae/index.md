writeCode

Write code to:-

- create a database named `sports`.
<!-- use sports -->
- list all databases present in local mongod server.
<!-- show dbs -->
- create 3 collections named `cricket`, `football`, `TT` in sports databse.
  <!-- db.createCollection('cricket') -->
  <!-- db.createCollection('football') -->
  <!-- db.createCollection('TT') -->
- add multiple players in those collections which should have fields like `name`, `age` and `email` and `bid_price`.
  <!-- db.cricket.insert( [{ name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4}, {name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4},{name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4}]) -->

  <!-- db.football.insert( [{ name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4}, {name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4},{name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4}]) -->

  <!--   <!-- db.TT.insert( [{ name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4}, {name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4},{name: "player1", age: 15, email: "email1@gmail.com", bid_price: 4}]) -->

- list all collections in sports database.
<!-- db.runCommand( { listCollections: 1.0, authorizedCollections: true, nameOnly: true } ) -->
- rename `TT` collection to `tennis`.
<!-- db.TT.renameCollection("tennis") -->

- create a capped collection called `khokho` which should have max 3 documents.
  <!-- db.createCollection( "khokho", { capped: true, size: 100000, max: 3 } ) -->

  Try inserting more than 3 and see what happens?
    <!-- db.khokho.insertMany([
     { item: "journal", qty: 25, tags: ["blank", "red"], size: { h: 14, w: 21, uom: "cm" } },
     { item: "mat", qty: 85, tags: ["gray"], size: { h: 27.9, w: 35.5, uom: "cm" } },
     { item: "mousepad", qty: 25, tags: ["gel", "blue"], size: { h: 19, w: 22.85, uom: "cm" } }
  ]) -->

<!-- db.khokho.insert({ item: "mousepad", qty: 25, tags: ["gel", "blue"], size: { h: 19, w: 22.85, uom: "cm" }}) -->

- check whether a collection is capped or not?
<!-- db.collection.isCapped() -->
- drop all documents from `football` collection.
<!-- db.football.remove( { } ) -->

- delete cricket collection completely.
<!-- db.cricket.drop() -->
- delete sports database.
<!-- db.dropDatabase() -->
- check which database you are connected to ?
<!-- db -->
- connect to test database
<!-- use test -->
