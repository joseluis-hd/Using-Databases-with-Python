**1. How do we model a many-to-many relationship between two database tables?**
```
  a) We add a table with two foreign keys
  b) We use a BLOB column in both tables
  c) We use the ARRAY column type in both of the tables
  d) We add 10 foreign keys to each table with names like artict_id_1, artist_id2, etc.
```
Answer is: _a) We add a table with two foreign keys_


**2. In Python, what is a database "cursor" most like?**
```
  a) A file handle
  b) A Python dictionary
  c) A method within a class
  d) A function
```
Answer is: _a) A file handle_

**3. What method do you call in an SQLIte cursor object in Python to run an SQL command?**
```
  a) run()
  b) send()
  c) socket()
  d) execute()
```
Answer is: d) execute()

**4. In the following SQL**
``` SQL
cur.execute ( SELECT count FROM Counts WHERE org = ? ', (org, ))
```
**what is the purpose of the "?"?**
```
  a) It is a search wildcard
  b) It is a placeholder for the contents of the "org" variable
  c) It is a syntax error
  d) It allows more than one boolean operation in the WHERE clause
```
Answer is: _b) It is a placeholder for the contents of the "org" variable_

**5. In the following Python code sequence (assuming cur is a SQLite cursor object),**
``` PYTHON
cur. execute ('SELECT count FROM Counts WHERE org = ? ', (org, ))
row = cur. fetchone ()
```
**what is the value in row if no rows match the WHERE clause?**
```
  a) -1
  b) An empty dictionary
  c) None
  d)An empty list
```
Answer is: _c) None_

6. What does the LIMIT clause in the following SQL accomplish?
``` SQL
SELECT org, count FROM Counts 
ORDER BY count DESC LIMIT 10
```
```
  a) It only retrieves the first 10 rows from the table
  b) It only sorts on the first 10 characters of the column
  c) It reverses the sort order if there are more than 10 rows
  d) It avoids reading data from any table other than Counts
```
Answer is: _a) It only retrieves the first 10 rows from the table_

**7. What does the executescript() method in the Python SQLite cursor object do that the normal execute() method does not do?**
```
  a) It allows database tables to be created
  b) It allows embedded JavaScript to be executed
  c) It allows multiple SQL statements separated by semicolons
  d) It allows embeded Python to be executed
```
Answer is: _c) It allows multiple SQL statements separated by semicolons_

**8. What is the purpose of "OR IGNORE" in the following SQL:**
``` SQL
INSERT OR IGNORE INTO Course (title) VALUES ( ? )
```
```
  a) It makes sure that if a particular title is already in the table, there are no duplicate rows inserted
  b) It ignores errors in the SOL syntax for the statement
  c) It updates the created _at value if the title already exists in the table
  d) It ignores any foreign key constraint errors
```
Answer is: a) It makes sure that if a particular title is already in the table, there are no duplicate rows inserted

**9. For the following Python code to work, what must be added to the title column in the CREATE TABLE statement for the Course table:**
```SQL
cur.execute (' ' INSERT OR IGNORE INTO Course (title)
  VALUES ( ? )''', ( title, ) )
cur.execute ('SELECT id FROM Course WHERE title = ?'
(title, )) 
course id = cur. fetchone () [0]
```
```
  a) A NOT NULL constraint
  b) A UNIQUE constraint
  c) An AUTOINCREMENT indication
  d) A PRIMARY KEY indication
```
Answer is: _b) A UNIQUE constraint_
