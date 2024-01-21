# Book Database with ISBN Searchability
This web application allows the user to save books they have read with ratings along with their
descriptions. It also allows the functionality for multiple users to add their own entries.

Editing and deleting entries can be done via the UI, but can only be done by the user who entered it.

This application is built using Node.js and MongoDB for persistence. Use npm install in the terminal to get
the node modules required to start. Statement npm run dev also runs nodemon so live updates are show instantly.

# Note
  - You will need to update the Google API link and create your own API key to run this application. You can change it in the books.js in the routes folder. You can get a key in Google Developer (where there is better documentation for creating one than here).

# Home Page
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/e8b1b970-1603-48f6-967a-58642452a813)
    - Front page populated with entries from previous users
    - UI changes depending on what user is logged in
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/eed6e78f-50a6-4ddd-bf78-c133c22302fb)
    - For this demo, the new user below is used
    - You can add a book now along with seeing prompts

# Register Page
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/65d7f140-0a05-4ea3-b2cd-9262ad0c36e3)
    - Form that registers the user with information given
    - It saves the user into the database with passwords hashed and salted using bcrpyt

# Login Page
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/b1027908-b68f-4ecc-9082-76323db2b0ba)
    - Form for login

# Book Page
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/d2260df3-7dfd-4af1-9696-df24383d833d)
    - Full Description of Book Page
    - Uses Google Books API with the ISBN to generate a deeper description along with its book cover
    - The delete and edit buttons on the bottom will redirect to home page as this user was not the one to enter this book

# Add Book Page
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/5ff55fbd-b5ae-4f7e-a44a-008f18064dd8)
    - Form to add book along with ratings
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/e8ab9de6-d3eb-4756-9d11-01cdfcea6bcd)

# Edit Book Page
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/0ab0c081-0732-44c3-9c3a-d48868fcad3a)
    - Clicking the edit button from this entry
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/f745d5a5-de18-4efb-a8c0-9e6c823d5b4e)
    - Changing the genres
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/53aaceb5-21ce-4c96-81b1-8b13c93224f7)
    - Updated entry on front page

# Search with ISBN Page
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/10383de5-2df4-4f23-8ff8-f7520bd8fa85)
    - Searching with random isbn number
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/e219a5c9-b5fd-4614-a89e-a8799474f1b6)
    - Result of random isbn number

# MongoDB Database Entries
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/4a77e93c-1022-40ed-8ab0-a16d5089ee11)
    - Table for book entries
  - ![image](https://github.com/brucebalutan/Book-Database-with-ISBN-Searchability/assets/19336369/9ad2c200-a66d-46f9-82ee-556b12f9855f)
    - Table for users
    - Note that password is encrypted

# Some Conclusions on the Project
  - Wanted to use pug/jade for practice
  - Not to happy with it, the styling with bootstrap does not work too well for pug (if at all)

