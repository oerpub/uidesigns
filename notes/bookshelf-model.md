# Bookshelf Model for Creating and Finding Book Repos

Because non-coder authors won't understand book repository, we are considering a "bookshelf" model. At the same time,
it is advantageous to use the term repositoryy in concert with shelf so that technical authors know how to find their books
on github or using git also.

## Screens

### Login
The login page needs to  have a way to select the book repo you want to open. 
Something like

**Sign in to the Book Editor**

[*author id*]  \[*password*\] ([or use advanced login with oauth](http://www.google.com))

[No thanks, I just want to demo](http://www.google.com) - This takes you to the demo book only.

[Sign in]

and then the next page:

**Choose Bookshelf**

[Start with the demo book](http://www.google.com)

or 

[*owner id*] [*bookshelf (repository) id*]  -- Eventually this can become the "Choose Bookshelf" menu illustrated
below under Change Bookshelf.

[Continue]

### Fork this book

Needs to ask you for a bookshelf id, prepopulated with the one that you are forking from. For now can always go to your
login account.

Cases

1. You are not logged in. -- Needs to ask you to login in to the account you want to fork the book into.
  * Use the new mockup*05 login screen, but remove "If you refresh ..." and remove "No thanks, ...".
2. You already have a fork of this book. -- Needs to say "You already have a copy of this bookshelf. [Take me there] [Cancel]."
3. You are logged in and you don't have a fork. -- Needs to ask you to supply an id for this bookshelf and supply the current id by default. "Please provide an ID for your copy." [current-id-by-default] Valid ids? - Hover says "You can use letters, numbers, and hyphens. Don't use spaces.") 
4. You have permission on the current book and thus get Save All instead of Fork. Just add a "Fork this book" in the dropdown under "Save All".

### Change bookshelf (book repository)

This should move to the Picker because that is a logical place for it. Connexions can hide this as they don't
need the functionality. 

Things to include
 * a list of recent bookshelves
 * a way to request a list of book repos in your account
 * a way to request a list of books in someone else's account (for now you have to know their id)
 * a way to specify both [owner id] [bookshelf id]

Selection of a different branch needs to be in an advanced thing and more hidden for now.

### Help things

"What is a book shelf / repository?" A bookshelf holds a single book or a set of related books that you want to edit at 
the same time and with the same co-authors. The books might share content; for instance a textbook student and teacher
editions. 
