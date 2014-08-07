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
#todo finish here
