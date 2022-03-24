---
1. As a user of the system I want to be able to see each store's offering and the amount of product in stock by square feet.
2. The application must allow employees to add new products to the system. As well as delete and edit them.
3. The different categories of floors available are tile, stone, wood, laminate and vinyl
4. The application must contain a database (DB) of floors.
5. Users must be able to search for products by picking from a hierarchical list, where the first level is the floor category, and the second level is the floor type.
6. Users must also be able to specify an item by typing its name (search functionality).
7. All floors regardless of their category have an associated color, size, brand, type and price
8. Categories tile and stone have different materials they are made of, e.g. Tile - porcelain, ceramic, resin; Stone - marble, pebble, slate
9. Wood floors have both a type (solid, engineered, bamboo, etc) and species (oak, hickory, maple, etc.)
10. Laminate can be regular laminate or water resistant, whereas vinyl can be water resistant or waterproof
11. The User Interface (UI) must be intuitive and responsive
---

## User class
- In requirements, There is no such thing as id or name, so we not going to have attributes
- In requirement 1, user are allow to see each store
- In requirement 5, user can search hierarchical list

## Store class
- Store is able to see whats offering and amount of product in stock by square feet
  - 2 attributes that is the product name and amount of product

## History class
- In requirement 5, Hierarchical list have floor category and floor type, and as hierarchical floor it should have product name, so History class will have a list attributes that have 3 element, and that is also can be use by search
- user can check history directly, history can be product in different store

## Search function class
- In requirement 6, Search is allow for users
- In requirement 5 we have to search by floor category and type, in requirement 6 we have to search by name, to make both working, Search class cover 3 attributes that is product name, floor category and floor type
- search for one product, and that can be same product name in different store
  - therefore we have a relation that 1 search for * product

## Employee
- has relation with store, one store can have many employee
  ## Edit class
  - Edit is only useable by employee for store that work in
    - contain function that able to edit product in store
    - requirement 2

## DB
- DB is where we have the "product" infomation, which cover requirement 4,7
- DB have FloorCategory class
- since is there is chance that same Product can have same name, add in ProductID to identify product

  ## FloorCategory class
  - include different Floor category
  - each FloorCategory have different FloorType
    - which cover requirement 3,8,9,10