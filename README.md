This is a simple web application for managing departments and employees. The web application uses the aforementioned web service for storing data and reading 
them from the database. The web application allows:

1. display a list of departments and the average salary (calculated automatically) for these departments
2. display a list of employees in the departments with an indication of the salary for each employee and a search field to search for employees born on a certain date or in the period between dates
3. change (add/edit/delete) the above data

The structure of the project is following:

Department-app (a project/app directory). It includes:    
  |__ migrations (includes migration files to manage database schema changes)  
  |__ models (includes modules with Python classes describing DB models)  
  |__ service (includes modules with functions/classes to work with DB)  
  |__ rest (this package must include modules with RESTful service implementation)  
  |__ templates (this folder must include web app HTML templates)  
  |__ static (this folder must include static files (js, css, images, etc,))  
  |__ tests (this package must include modules with unit tests)  
  |__ views (this package must include modules with Web controllers/views)  
  
To read extended information describing usability of project open the [SRS.md](SRS.md) file.
