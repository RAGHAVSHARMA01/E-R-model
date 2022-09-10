#  E-R Model 
---
> E-R stands for the entity relation model.It is a high-level data model. This model is used to define the data elements and relationship for a specified system.In other words we can say that the E-R model is the conceptual model by which you can convieve the structure of database, maintain relationships between componetn & identify the constraints that occure in the integrated design of the complete database system.
>
> There are 3 components of the E-R model
>   - Entity
>   - Attribute
>  - Relationship
 >  
> ### Entity - 
>Layman would say this as real worl object that can be differential and guess what this is the meaning of the Entity for any technical person also for the common understanding.
>    Example would make thing easy to understan like we can say Book is a **Entity set** and the DBMS book will be a **entity**
>    - **Entity Set** - Collection of the entities that can share similar properties can be considered as the entity set.
>
>  ![Image of the entity and attribute](https://github.com/RAGHAVSHARMA01/E-R-model/blob/main/1.png)   
>
> ### Attritute - 
> There are the properties that can be used to express any entity or the entity set or any physical thing for that matter is the attribute of the formal.
>
> OR 
>
> Attritube is a specific part of the Entity that is used to give its properties. Saying technically, it is the mapping from a entity set to its **domain value**
> 
> There are 5 types of Attribute
> - Single value attribute :- Those value that containt only only value, eg:- addhar card ( one for every person) ,Age ,Driving Licience
> - Multivalued Attribute :- When we have more than one value for a single entity, eg:- Phone number, Clothes, etc
> - Composite Attribute :- Those attribute which can be further divided, eg :- A very good example could be NAME = First + Middle + Last
> - Atomic Attribute :- Those attribute which can be no more further divided, eg:- surname
> - Stored Attribute :- Lets understand this by taking an example today is 10th september,2022 and D.O.B of a persom is 18th March,2001 then it is easy to say that the age of the person is 21years, this age is known as stored attribute or the derived attribute
> ### Relationship - 
> A relationship is the association amoung several entities denoted by the diamond.
> 
> There are 3 types of relationships
>   - One to One :- (also denoted as 1:1) This is the least common type of relationship in a data model. It’s a relationship where a record in one entity (table) is associated with exactly one record in another entity (table), eg:- Country and capital city, Husband and wife (at one time)
>   - One to Many :- (also denoted as 1:M) It is the most common type of relationship, where a record in one entity can be referenced by multiple records in another entity, eg:- Employee - manager: Each employee has exactly one immediate supervisor or manager, but each manager usually supervises many employees, Parent and children:
> - Many to Many :- (also denoted as N:M) When more than one instances of an entity is associated with more than one instances of another entity then it is called many to many relationship. For example, a can be assigned to many projects and a project can be assigned to many students.
>
>### *Undersatanding Degree of E-R model, Cardinality ratio, Participation or Existence, Different representation of relationships w.r.t different relationships*
>
> #### ONE TO MANY RELATIONSHIP - 
> LET's take a example that every employee works for exactaly one department and the department can have more than one employees,  New deparrtment need not to have any new employee
>
> ![Image of a one to many relationship](https://github.com/RAGHAVSHARMA01/E-R-model/blob/main/o%20to%20m.png)
>
>   - Degree of ER model -> Number of entities participating in an relationship is known as degree. IN this case 2 entitie are there one is employee and the other is department so the degree here is 2
>   - Cardinality Ratio -> Max. number of time entity can participate in the relationship. This should be calculate foe each entity in participation. In the example here the cardinality ratio of employee is 1 and the cardinality ratio of teh department is 2 as d2 have two employee e1 and e2 in his department
> - Participation or Existence -> Min. number of times entity can participate in a relationship. In the example above employee has participation as 1 and the deaprtment has 0 participation because d4 has no employee in it
>    * whenever the entity have his/her participation as non-zero we call it as a total participation(represented by the double line or the dark line)  and when the entity has the participation as non zero then we call it as the particial participation(represented by the single line).
> 
> **Note**
>  Cardinality Ratio and Participation are combinally known as **structural constraint**
>
> #### ONE TO ONE RELATIONSHIP - 
>
> ![image of one to one relationship](https://github.com/RAGHAVSHARMA01/E-R-model/blob/main/o%20to%20o.png)
>
>
> LET's take a example that every department should have a manager and only one employee will manage one department (employee can manage only one department)
> - Degree -> Here the degree would be 2
> - Cardinality Ratio -> Employee has 1 and department also have 1
> - Participation or Existence -> Employee has it as 0 ( partial) and department has it as 1 ( total)
> #### MANY TO MANY RELATIONSHIP -
>
> LET's take a example that every project have atleast one Employee and every employee has atleast one project then
>
>  ![image of one to one relationship](https://github.com/RAGHAVSHARMA01/E-R-model/blob/main/m%20to%20m.png)
>  ```
> - Degree -> Do it Your self 
> - Cardinality Ratio -> Do it yourself
> - Participation -> Do it yourself
> ```
>
> ---
> #### Strong Entity and Weak Entity
>  Those entites which can be identified with its own attributes **uniquely** are known as Strong entities 
>  Those entites which need to be dependend on other attributes to be identified **uniquely** are Weak entities
>
> **Note**
>   Strong entites have their own primary key, Participation of the weak entity will always be Total 
>
> *By - Raghav*














