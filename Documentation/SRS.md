
## 1. Departments
##### Display list of department
This mode is intended for viewing and editing the departments list 

___Main scenario:___ 
* User selects item “Departments”; 
* Application displays list of department. 

![1](https://user-images.githubusercontent.com/65542353/127387862-ace08915-3504-4c30-b775-319e18a02409.png)

The list displays the following columns: 
* Department name – departament name; 
* Average salary – Average wages of employees; 


##### Add department
___Main scenario:___ 
* User clicks the “Add” button in the department list view mode; 
* Application displays form to enter department data; 
* User enters department data and presses “Save” button;
* If any data is entered incorrectly, incorrect data messages are displayed; 

![eror_incorect](https://user-images.githubusercontent.com/65542353/127707104-5f1cc988-e42d-478a-a31e-90e1a7cc3a2f.png)

* If entered data is valid, then record is adding to database; 
* If error occurs, then error message is displaying; 

![adderr](https://user-images.githubusercontent.com/65542353/127623054-bbb46552-5e15-42a8-9fc1-4cd6db64c6dd.png)

* If new department record is successfully added, then list of department with added records is displaying. 
Cancel operation scenario: 
* User clicks the “Add” button in the department list view mode;
* Application displays form to enter department data; 
* User enters department data and presses “Cancel” button;
* Data don’t save in data base, then list of department records is displaying to user. 
* If the user selects the menu item ”Department” or "Employee", the data will not be saved to the database and the corresponding form with updated data will be opened. 

![2](https://user-images.githubusercontent.com/65542353/127388666-6bee0a67-c101-4f5c-a217-d147a66aa396.png)

When adding a department, the following details are entered: 
* Department name – departament name; 

Constraints for data validation:

* Department name – maximum length of 30 characters; 
* Average salary- maximum length of 5 characters; . 
 ##### Edit department
___Main scenario:___ 
* User clicks the “Edit” button in the department list view mode; 
* Application displays form to enter department data;
* User enters department data and presses “Save” button; 
* If any data is entered incorrectly, incorrect data messages are displayed; 

![Edit_incorect](https://user-images.githubusercontent.com/65542353/127707610-40d1cf15-d71f-40d3-bf68-01d002988429.png)

* If entered data is valid, then edited data is added to database; 
* If error occurs, then error message is displaying; 

![editerr](https://user-images.githubusercontent.com/65542353/127623114-dfcbe175-3ad4-457f-b636-5ee2f2a22282.png)

* If the departments record is successfully edited, the list of departments with the added records is displayed and the data in the "depatments" table is changed.

![редактировать](https://user-images.githubusercontent.com/65542353/127388771-dee34b02-ea34-49c5-9511-cdb05d5894e1.png)

If the user selects the menu item ”Departments” or "Employees", the data will not be saved to the database and the corresponding form with updated data will be opened.


##### Removing the department
___Main scenario:___ 
* The user, while in the list of departments mode, presses the "Delete" button in the selected department line; 
* Application displays confirmation dialog “Please confirm delete department?”; 
* The user confirms the removal of the department;
* The user confirms the removal of employees of this department; 
* Record is deleted from database; 
* If error occurs, then error message displays; 

![err](https://user-images.githubusercontent.com/65542353/127623171-73bc29b8-388f-4d7b-ac23-aa9d82a2664b.png)

* If a department record is successfully deleted, a list of departments with no deleted records is displayed and employees with the deleted department are deleted.

![удалить](https://user-images.githubusercontent.com/65542353/127388802-c8d1113f-3bb6-4fa5-b2ad-f5633a0da100.png)

___Cancel operation scenario:___
* User is in display mode of departments list and press “Delete”,“Edit”, “Add” button; 
* The application displays the selected window; 
* User press “Cancel” button; 
* List of departments without changes is displaying. 

## 2. Employees  
  ### 2.1. Display list of Employees  
  This mode is intended for viewing and editing the employees list.  
  
  __Main scenario:__
  1. User selects item "Employees";
  2. Application dispalys list of employees.  
      
  ![image](https://user-images.githubusercontent.com/83345134/127887980-21df5e37-3439-4cb9-930a-9b301fca292d.png "Employees list")  
    Pic 2.1.1 View the employees list.
    
  __The list displays following employees' information:__  
  1. Department - place, where employee is working;  
  2. Name of the employee;  
  3. Date of birth of the employee;  
  4. Employee's salary.  
   
  __Filtering:__ 
  1. In the employees list view mode, the user can combine date filter and department filter: he/she sets a date, choose any existing department and presses the    refresh list button (to the right of the date entry field);  
  2. The default value of department filter is null, so user can skip setting this filter to get all employees. 
  3. The application will show only filtred employees.
  4. If user wants to get employees, that are born below any date, he/she should set only end date and press refresh button.
  5. If user wants to get employees, that are born after any date, he/she should set only start date and press refresh button.
  6. To reset filter, user should press the reset button.
  7. The example of filter is following:  
  ![image](https://user-images.githubusercontent.com/83345134/127888106-4d4df459-eb8b-4654-94fa-e85cdb06e567.png)  
  Pic 2.1.2 Filtering example

  __Restrictions:__  
  * Start date of the period should be less then end date of the period, but if the user will make a mistake, he/she will see the invalid date message  
  ![image](https://user-images.githubusercontent.com/83345134/127888024-4d0cafb2-8566-4157-8657-7cb3a01118c6.png)  
  Pic 2.1.3 Invalid date message
  * Updating data after selecting the filtering conditions is carried out by pressing the “Refresh” button.  

      
  ### 2.2. Add employee  
     
   ![image](https://user-images.githubusercontent.com/83345134/127285174-8b015c12-a1b2-4ff9-a32c-d93a516a4bbb.png "Add employee")  
      Pic 2.2.1 Add employee.  
      
  __Main scenario:__  
  * User clicks the “Add” button in the employees list view mode;  
  * Application displays form to enter employee data;  
  * User enters employee’s data and presses “Save” button;  
  * If any data is entered incorrectly, incorrect data messages are displayed:  
  ![image](https://user-images.githubusercontent.com/83345134/127649375-0ce328e1-11a7-494b-a3c3-54e2081a6185.png)  
  Pic 2.2.2 Adding validation error  
  * If entered data is valid, then record is adding to database;  
  * If error occurs, then error message is displaying, the message is following:  
  ![image](https://user-images.githubusercontent.com/83345134/127639007-3ceae0d9-212e-4714-8424-e515f535e0e3.png)  
  Pic 2.2.3 Adding system error  
  * If new employee record is successfully added, then list of employees with added records is displaying.   
      
  __When adding a employee, the following details are entered:__  
  * Department – employee’s work place;  
  * Name – employee’s name;  
  * Salary – employee’s salary;  
  * Date of birth – employee’s date of birth.  

  __Constraints for data validation:__  
  * Department – one of the departments;  
  * Name –  maximum length of 45 characters;  
  * Salary – maximum value is 2000;  
  * Date of birth – date in format dd/mm/yyyy.   
      
  ### 2.3 Edit employee  
        
![image](https://user-images.githubusercontent.com/83345134/127285373-3f14cb74-9510-4dc3-8e3a-2c2c01dee4a4.png "Edit employee")  
    Pic. 2.3.1 Edit employee.  
    
  __Main scenario:__  
  * User clicks the “Edit” button in the employees list view mode;  
  * Application displays form to enter employee data;  
  * User enters cemployee’s data and presses “Save” button;  
  * If any data is entered incorrectly, incorrect data messages are displayed  
  ![image](https://user-images.githubusercontent.com/83345134/127649385-d249277f-5c6b-499c-bfdc-eb31d32e981a.png)  
  Pic 2.3.2 Editing validation error  
  * If entered data is valid, then edited data is added to database;  
  * If error occurs, then error message is displaying  
  ![image](https://user-images.githubusercontent.com/83345134/127639014-e66fa490-4b0f-487c-8006-6faf4f215ced.png)  
  Pic 2.3.3 Editing system error  
  * If employee’s record is successfully edited, then list of employees with added records is displaying.   

  ### 2.4 Removing employee  
        
  ![image](https://user-images.githubusercontent.com/83345134/127890749-2785e253-ff3d-4d9c-94e3-46be05d34c25.png)  
    Pic 2.4.1 Delete employee dialog.  
    
  __Main scenario:__  
  * The user, while in the list of employees mode, presses the "Delete" button in the selected employee line;  
  * Application displays confirmation dialog “Please confirm delete employee?”;  
  * The user confirms the removal of the employee;  
  * Record is deleted from database;  
  * If error occurs, then error message displays  
  ![delete error](https://user-images.githubusercontent.com/83345134/127890943-82714496-3ffd-4102-a647-64cd25345d8b.png)
  Pic 2.4.2 Deleting error occurs   
  * If employee record is successfully deleted, then list of employees without deleted records is displaying.     
    
   ### 2.5 Canceling operation
   If user wants to cancel Adding/Editing/Deleting operation, there are several ways:
   * User can press button "Cancel", then user will be returned to employees list;
   * User can switch to "Departments" menu item and chnges won't get in database.

