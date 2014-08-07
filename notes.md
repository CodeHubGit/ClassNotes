#codehub.io class notes

##Creating an Application
* User Story (no programming language)
 * describe parts of application from the perspective of the user
 * **EX** "As a user, I want to play a game that will prompt me to go left or right."
* Design Doc  (basic coding language or "psuedocode")
 * developer perspective of how to build what the user is going to do
 * **EX** in order to do this, I'm going to need a function to handle the fight aspect...
* Comments in Code (more specific coding terms and instructions)
 * Helps guide code writing
 * **EX** Here I'm going to define a function and it will take these variables and define values
* **Note: Continually Update these as you change your program**
* 

##Key Terms
* Frontend
 * **Browser**, **HTML**, **JS** and **CSS**
  * Run and compiled on browser locally (always retrieving the newest thing)
* Backend
  * **Server**
   * Always active - don't kill it like we do the browser
   * Keeps track of user account info and other data
   * If server goes down, lots of problems with data will occur unless a database is used
* Node.js
  * server layer, can host http easily, network communication, run in js, works nicely with MongoDB and other databases
  * npm - **n**ode **p**ackage **m**anager
* Database - db (**EX** mySQL, MongoDB)
 * **ACID** (most conform to this)
  * **A**tomic, **C**onsistent, **I**solation, **D**urability
    * Atomic
     * no half-reads or writes (no corrupted data)
     * completes or does nothing
     * compresses to small format
     * read and write quickly
     * difficult to crash
 * SQL
  * Any database that takes SQL (**s**tructured **q**uery **l**anguage
   * ' where username = "alex" ' - returns data that fits given command)
   * every db has own commands
    * problem: if db is updated, old code will break
* ORM - **O**bject **R**elational **M**odel
 * someone wrote code that will generate SQL code for you
  * important for when db is updated
* noSQL  -->  Doesn't take SQL but JavaScript
 * **EX** MongoDB or Couch Database
 * 100x slower for writing than SQL but 100x faster for readings
  * Most applications read more than write, so a write-heavy app needs SQL
* CRUD - **C**reate **R**ead **U**pdate and **D**elete - 4 main db operations

##What is good code?
* Highly modular - one piece works in a lot of places and can work in other code
 * **EX** libraries are very modular
* Separation of Concerns (SoC) - non-overlapping interests, different functions deal with different parts of code
* Design patterns - common patterns that apply to diff programming languages and frameworks
* DRY - **D**on't **R**epeat **Y**ourself - do it right the first time so you don't have to change it anywhere else
* Conventions - patterns that community has decided is the best way to write code, not enforced by language

##Design patterns
* Model View Controller -> **MVC** (most used in class)
 * model = raw data
 * view = user interface (HTML, CSS on front end, API on backend)
 * controller = layer that translates between model and view  --> takes action
  * routes = endpoints - user view of server functionality
   * most of the time we don't want the model and view to talk to each other (modular, SoC)
   * **EX** following this pattern means db could be swapped out from Mongo to mySql and view would not have to change
  * API - **A**plication **P**rogramming **I**nterface (new method of program communication)
   * JSON - **J**ava**S**cript **O**bject **N**otation - format of data sent over the web
  * **REST**ful - how we interact with APIs
   * get (recieve)
   * post (create)
   * put (update)
   * delete (remove)
   * Similar to CRUD but for apis
**VIEW**    **Controller**    **MODEL**
**frontend** -- **Api** -- **backend**

##todo finish here
