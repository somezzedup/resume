1. As a user of the system I want to be able to see each store's offering and the amount of product in stock by square feet.
-- This is achieved by creating a Store class, the user finds out each store's offering and the amount of product and price of per feet through calling the GetProduct method in the Store class from the database. 
2. The application must allow employees to add new products to the system. As well as delete and edit them.
-- In the Employees class, it provides AddProduct, EditProduct, and DeleteProduct methods to handle this requirement. However, To avoid administrative chaos, employees can only operate on the products of the respective store.
3. The different categories of floors available are tile, stone, wood, laminate and vinyl
-- Create multiple class which call tile, stone, wood, laminate and vinyl
4. The application must contain a database (DB) of floors.
--Create a database to store floor. As development progresses, different forms may be added to improve the software design. For example, order table, employees table and customer table.
5. Users must be able to search for products by picking from a hierarchical list, where the first level is the floor category, and the second level is the floor type.
--This was implemented by creating classes called Type and Catewgory. 
6. Users must also be able to specify an item by typing its name (search functionality).
-- Search for item can be integrated into one method. which calls SearchName()
7. All floors regardless of their category have an associated color, size, brand, type and price
--In the floor class, there are multiple attributes that implement this requirement.
8. Categories tile and stone have different materials they are made of, e.g. Tile - porcelain, ceramic, resin; Stone - marble, pebble, slate
9. Wood floors have both a type (solid, engineered, bamboo, etc) and species (oak, hickory, maple, etc.)
-- The type and material attributes are create by  Floor class. 
10. Laminate can be regular laminate or water resistant, whereas vinyl can be water resistant or waterproof
--There are IsWaterResostant and IsWaterProof two menthod to determine the floor water repellency.
11. The User Interface (UI) must be intuitive and responsive.
--Not considered because it does not affect the design directly.