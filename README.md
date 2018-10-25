# alumniOverflow

# TODO:
  * Design Database [Christian, Kyle].
  * Fill out TODO

# SETUP
  * Install SQLite
  * To access database, in "database" directory, type the following:
    ```
    sqlite3 2468
    ```
    This will create a database file "2468" in the database directory

# DATABASE
  * Create/enter the database called "2468" by typing the following command
    ```
    sqlite3 2468
    ```
  * To test, for now, do the following:
    * From the "database" directory, enter "sqlite3 2468" database
    * Execute ".read createschema.sql" to create tables
      * Should display "CREATE TABLE" 8 times.
    * Try inserting and deleting various things in the database
    * When finished, remove all data and drop tables by executing ".read dropschema.sql"
  
  __TO DO [Tanner, Christian, Jared]:__
  * Add keys
  * Connect to Python
  * Write scripts for incremental database design
  * Modify to make Q4 its own table (instead of the whole survey) -- for future, add tables for other questions as well
  * Create a test dataset
  * Make an automated test

# HTML TEMPLATES
Currently a few skeleton templates for the html files which we will need to make
  * survey_q#.html
    * the #th page which a visitor will view while taking a survey (can also most likely be put in a single file, but needs JavaScript
  * editor.html
    * the page for an editor to edit and publish new questions
  * answer.html
    * the page for responders to answer questions
  * responses.html
    * the page for viewing responses
