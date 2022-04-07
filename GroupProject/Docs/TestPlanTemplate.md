# Test Plan

**Author**: \<Bing gao\>

## 1 Testing Strategy

### 1.1 Overall strategy

We will start with unit testing then Integration Test. If the building is correct then we will move forward to system, regression and API testing in order.
 
1. Check if the user has access to the store.
2. Check if the user/employee are able to add, delete the material.
3. Check if the search system is working.
4. Check if the categories are divided perfectly. 

### 1.2 Test Selection

Black Box:System Testing (software specification)
1. Log on as a user
2. Log on as a employee
3. Search floor by store name as a user and employee
4. Search floor by floor name as a user and employee
5. Search floor by hierarchy(category and type) as a user and employee
6. Check the search search results 
7. Edit a floor information as an employee
8. Add a floor as an employee
9. Delete a floor as an employee
 
White Box:Unit testing & integrated testing (code)
1. Login
2. SearchStore
3. SearchFloorName
4. SearchCategory
5. SearchType
6. AddFloor
7. EditFloor
8. DeleteFloor


### 1.3 Adequacy Criterion

To ensure a list of good quality test case, we will select cases that cover every function of the application, i.e. every structure must execute at least once.

### 1.4 Bug Tracking

Unit Testing: Test each component is working properly, if it does not work or caused an error, we should refine code and make sure the component works properly
 
Integrated testing: Test components can interact with each other properly. Although each component is unit tested, there still exist defects for some reasons. The error occurs from the interface of the software modules with the database, Inadequate exception handling could cause issues.
 
System testing: System Testing is performed after the integration testing and unit testing. Check for errors by running the entire application. 

### 1.5 Technology

JUnit(API)

## 2 Test Cases

|Test Description |Test Case ID |Test Case Action |Test data(Input) |Expected Output |Actual Output |Test Status(Result)|