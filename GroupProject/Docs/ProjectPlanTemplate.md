# Project Plan

**Author**: \<Jiawen Lin\>

## 1 Introduction

A software that allows users to search for flooring products from different stores

## 2 Process Description

    Activity name: Search
    Activity description: Search products with 1 to 3 attributes of the product, which are product name, floor category, and floor type. For different floor categories, we can have different floor types, so to search by floor type, the user must select one of the floor category from (Tile, Stone, Wood, Laminate, Vinyl). Which floor category is the first level, after picking from the floor category, the user can pick second-level choices. For example, the user picks Stone as the floor category, then the user can pick (marble, pebble, slate) as the floor type. If a user only picks first-level search, but not second-level, the result of the search can have different floor type products with the same floor category.
    Entrance criteria: Product name, floor category, floor type
    Exit criteria: 

    Activity name: search_result
    Activity description: After Searching, this activity will have the product list that matches the searching
    Entrance criteria: Product name, floor category, floor type
    Exit criteria:
    
    Activity name: floor_infomation
    Activity description: every product have its floor information page, which displays all information about a product (product name, floor category, floor type, color, size, price, brand)
    Entrance criteria: 
    Exit criteria:
    
    Activity name: login
    Activity description: user will need to log in to use the history that has been saved, if the user is not login, the history activity will not be useable
    Entrance criteria: Username, password		// 
    Exit criteria: 
    
    Activity name: history
    Activity description: Users who log in can use history to view the hierarchical list of floors that are viewed in the history
    Entrance criteria: user can be identified by username or user id for every user if needed
    Exit criteria: output list of floor products as the result
    
    Activity name: employee_edit
    Activity description: employee can edit products where the employee works, that account needs store information, such as store id, store name, user account can be upgrade into employee account by proof of identity
    Entrance criteria: store id, username, password
    Exit criteria:


## 3 Team


    - Mezbahuddin Prottoy
    - Bing Gao
    - Muhammad Zair 
    - Kamal Gurung
    - Jiawen Lin

    - Project Manager: - The role of the project manager is to ensure that the project is working fine and everyone in the team functions accordingly and on time. It also ensures that the whole team is working as one unit.
    - Frontend Developer: Is responsible for working on designs and layouts and implementing GUI.
    - Backend Developer: Creates the functionality specified in the application requirements. Utilizes the database and CRUD functions to push accurate data to the frontend components.
    - Database Engineer: Engineer: Constructs and maintains the database. Creates CRUD functionality to fulfill requirements.

    - Mezbahuddin Prottoy: Database
    - Bing Gao: Project  backend
    - Muhammad Zair : Frontend
    - Kamal Gurung : Backend
    - Jiawen Lin : Project Manager
