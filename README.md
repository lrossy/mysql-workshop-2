# MySQL Workshop 2 - Basic Data Manipulation

## Workshop Contents

### Data Manipulation Statements

* [Insert](http://dev.mysql.com/doc/refman/5.7/en/insert.html)
* [Update](http://dev.mysql.com/doc/refman/5.7/en/update.html)
* [Delete](http://dev.mysql.com/doc/refman/5.7/en/delete.html)

### Data Manipulation Queries

* [Select](http://dev.mysql.com/doc/refman/5.7/en/select.html)
  * [Count](https://dev.mysql.com/doc/refman/5.7/en/counting-rows.html)

### Query Clauses

* [Limit](http://dev.mysql.com/doc/refman/5.7/en/limit-optimization.html)
* [Where](https://dev.mysql.com/doc/refman/5.7/en/where-optimizations.html)
  * [Logical And Operator](https://dev.mysql.com/doc/refman/5.7/en/logical-operators.html#operator_and)
  * [Logical Or Operator](https://dev.mysql.com/doc/refman/5.7/en/logical-operators.html#operator_or)
  * [Like Operator](https://dev.mysql.com/doc/refman/5.7/en/string-comparison-functions.html#operator_like)

### Query Modifiers

* [Order By](http://dev.mysql.com/doc/internals/en/optimizer-order-by-clauses.html)
* [Group By](http://dev.mysql.com/doc/internals/en/optimizer-group-by-related-conditions.html)


### MySQL Bulk Data Import
```
# Executing Statements from an External File
mysql> source <filename>
```

## Workshop Instructions

* Fork this repository
* For every exercise in this Workshop:
  * Create a new file named "exercise-n.txt", containing:
    * The SQL Statement used, when applicable
    * The SQL Statement results, when applicable
* After the first exercise you commit, do a pull request from your master branch. Then, commit and push after each exercise so that we can see your progress.

### Exercise 1
* Import Database Schema from the following source file into ```decodemtl_addressbook```:
  * data/import-table-structure.sql

### Exercise 2
* Insert one row into ```decodemtl_addressbook.Account```
* Insert one row into ```decodemtl_addressbook.AddressBook```
* Insert three rows into ```decodemtl_addressbook.Entry```

### Exercise 3
* Retrieve data from the previously inserted ```decodemtl_addressbook.Account``` row
* Retrieve data from the previously inserted ```decodemtl_addressbook.AddressBook``` row
* Retrieve data from the previously inserted ```decodemtl_addressbook.Entry``` rows

### Exercise 4
* Modify the ```decodemtl_addressbook.Account``` row
* Modify the ```decodemtl_addressbook.AddressBook``` row
* Modify the three ```decodemtl_addressbook.Entry``` rows using one query only

### Exercise 5
* Delete all data from ```decodemtl_addressbook.Entry``` without using a ```DELETE``` statement

### Exercise 6
* Delete ```decodemtl_addressbook.Account``` and all associated date

### Exercise 7
* Import Database Schema from the following source file into ```decodemtl_addressbook_import```:
  * data/import-table-structure.sql
* Bulk import data from the following source files into ```decodemtl_addressbook_import```:
  * data/import-account.sql
  * data/import-addressbook.sql
  * data/import-entry.sql

### Exercise 8
* What is the email of the Account identified by "63"?
* What are the names of the AdressBooks belonging to accountId "3"?
* On which date was the AddressBook titled "Lorem Foundation" created?

### Exercise 9
* How many Accounts exist?
* How many Address Books exist?
* How many Address Book Entries exist?

### Exercise 10
* How many Address Book Entries are listed as born before February 12th of 1982?
* How many Address Book Entries are listed as born on or after January 1st of 1965?
* Which Address Book Entry is listed as being the oldest of age?

### Exercise 11
* How many Address Book Entries are not listed as ```other```?
* How many Address Book Entries are listed as either ```home``` or ```work```?
* How many Address Book Entries are listed as ```phones```?
