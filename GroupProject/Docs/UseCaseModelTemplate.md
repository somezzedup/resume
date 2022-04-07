# Use Case Model

**Author**: \<Bing Gao\>

## 1 Use Case Diagram

*This section should contain a use case diagram with all the actors and use cases for the system, suitably connected.*
![alt text](CaseDiagram.png)

## 2 Use Case Descriptions

*For each use case in the use case diagram, this section should contain a description, with the following elements:*

- Guests can login to the APP only through login, Identify guests by identifying user information. User and Employee have two different views to operate. Users can search the floor through two methods (SearchCategory and SearchName) after SearchStore. SearchCategory will be designed as hierarchical. Employees can perform four operations on the store they are in , for example, Edit, Add, Delete and Read.
- You can perform the following operations only after logging in. Only employees can add, delete, edit the floors. User has only the permissions to search.
- Employees can edit and delete the floor under the floor information page. SearchType can only work after selecting SearchCategory.
- Guests are identified through the login page, then differentiate between employees and users based on login information. Assuming that the user is logged in, they can enter the name of the store to display all floor information for the store. In addition, the user also has two ways to conduct a more detailed search, which are to search floor by floor name and to search floor by hierarchy(category and type). Employees can perform not only all user operations, but also CRUD the store they are in.  