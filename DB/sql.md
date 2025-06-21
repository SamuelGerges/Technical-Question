## Database languages
    which includes the languages used to create, 
    manage, manipulate, and retrieve data from databases. 
    The most common and widely used database language is SQL (Structured Query Language).

    # Data definition language (DDL)
        - Used to create or modify the structure of the database.
        - Commands:
            CREATE: create tables, views, databases, etc.
            ALTER: modify existing table structure 
            DROP: delete a table or database
            TRUNCATE: remove all records from a table quick 

    # Data manipulation language (DML)
        - Used to manipulate data in the database.
        - Commands:
            SELECT: retrieve data
            INSERT: add new records
            UPDATE: modify existing records
            DELETE: remove record
    # Data control language (DCL)
        - Used to control access and permissions.
        - commands : 
            GRANT: give permission to users
            REVOKE: remove permissions

    # Transaction control language (TCL)
       - Used to manage transactions, ensuring data consistency.
       - Commands
            COMMIT: save changes
            ROLLBACK: undo changes  
            SAVEPOINT: mark a point in transaction
            


## Database SQL

### View
    it is a virtual table based on the result of a SQL query.
    It does not store data itself but shows data from one or more real tables.
    # advantage 
        - simplifies complex SQL logic
        - Improves security by hiding sensitive data
        - Provides data abstraction for different users
        - Reusable across multiple queries or applications
    # disadvantage
        - Performance issues if the view is based on complex queries
        - Cannot always update data through a view (especially with multiple tables or aggregates)
        - Dependency issues: Dropping a table that a view depends on will break the view
        

       
### Function
    it  is a set of SQL statements that perform a specific task and
    return a single value or a table (in case of table-valued functions).
    # advantage
        - Code Reusability – define once, use many times.
        - Modularity – makes large queries more manageable (تنظيم الكود).
        - Consistency – ensures that logic remains the same across the application.
        - Custom logic – allows implementing domain-specific calculations.

    # disadvantage
        - Performance: Scalar functions (return single value) can slow down large queries.
        - Limited access: Some functions can't modify data (unlike procedures).
        - Not index -friendly: Using functions in WHERE clause may prevent index usage.
        - Complexity: Overusing functions can make debugging difficult.
