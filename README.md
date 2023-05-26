# <div align="center">  Electronic Class Register </div>
###	We want to design a database that allows you to record the grades given to students. One of the basic tasks at the stage of database design is to define the basic objects in the field for which we design the database. In our case, we will quickly come to the conclusion that our database should describe students and the basic organizational unit of the school and class.
We can assume that a database designed in this way will act as a place where data is collected ratings will be provided.

----------------------------------------------------------------------------------
###	<div align="center">Installing Dependencies   </div> 
*	Use your favourite DB client.
*	Scripts included in the **[SQL Folder](https://github.com/HmSalah/COVID_case_tracker/tree/main/SQL)**

-----------------------------------------------------------------------------------	
##	<div align="center"> Database Modeling Process </div> 	 ##
1.	**Requirements Gathering**
		- Created a Statement of Requirements by summarizing user requirements
	
2.	**Building a Conceptual Model**
      - Provided a high-level overview of Electronic Class Register. 
	
3.	**Building a Logical - Physical Model**
      - Using favourite DB client, I created a Logical Model by defining the entities and relationships.
	*	Inserted primary keys and foreign keys.

We will now explain some elements of the proposed solution.
- Each table must have a name assigned to it and this name should define the type of data that we plan to store in this table.
- According to the characteristics of the relational model, each table must contain a primary key. For the proposed tables, the primary keys are the columns with the names id_student, id_mark, id_type_of_mark, id_teacher, id_school_subject and id_class.
- The purpose for which we design tables of this type seems obvious - we will use the primary keys from these tables as foreign keys in other tables containing information about the subject or type of assessment and thanks to this approach we will ensure the unambiguity of the stored data.


-----------------------------------------------------------------------------------	
##  <div align="center">  1- Statement of Requirements 

###### <div align="center"> This summary of all users’ requirements.</div>

* **Mark:**
    - id_student
  - id_teacher 
  - id_type_of_mark
  - id_school_subject
  - mark
  - date 
  - id_mark

* **Students:** 
  - id_student 
  - lastname 
  - name 
  - date_of_birth 
  - pesel_number 
  - id_class

* **Class:**
  - id_class 
  - name 
  - school_year

* **Types of marks:**
  - id_type_of_mark 
  - name

* **Teachers:**
  - id_teacher 
  - lastname 
  - name 
  - company ID 
  - professional_title

* **School subjects:**
  - id_school subject 
  - name

##  <div align="center"> 2 - Database schema model </div>
####    <div align="center">   A detailed description of the possible Entities & Attributes </div> 
<p align="center">  <img src="https://raw.githubusercontent.com/mrsaldona/electronic_class_register_sql/main/diagrams/Electronic_Class_Register_Schema.PNG" /></p>



