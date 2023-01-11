# Project 1
BOOK REVIEW WEBSITE

Web Programming with Python and JavaScript!

#video link=https://youtu.be/q9-YHV7Ndqk


::-api key= 4F8jNRtlEyCAZDu4iOVsw
::-DATABASE_URL=postgres://kidgbiaramncot:e27aacd8effa7ed84a73a1c02df17afbe4d3b85008bfdff0db4a99a2b2ee1df1@ec2-3-211-48-92.compute-1.amazonaws.com:5432/d1uhdgce03r14i

::-application.py is a main app file. Contains routing to all html files , queries to database and all other functions.
helpers.py contains one function , checks if there is data in session, if no data found redirect to log in page. 
import.py creates 3 tables:- users, reviews and books. After books are created it read csv file and loads all books skipping the first line (title row).

::-When you start my app first time you will be redirected to login page where you can register and log in,
"login.html" file extends layout.html. Threre are two forms in login page, one for registering and second for logging in.#One and only javascript function check if passwords match durign registration process. Existing users also is checked before registration.Succesfully registered you can try log in,if password or username do not match ,it will show "Wrong email or password. Try again."

::-User is redirected to index.html after logged in. If you requested index by GET , you will see simple quote and will be able search books database. If you request index by POST (searching for books) list of books shows. Clicking one of the book takes you to book.html (bookpage)

::-book.html file extends layout.html. On bookpage author, year and isbn are loaded. Also from goodread.com API rating count and rating itself are loaded. Also all reviews received from users along with ratings are loaded one under one. On the bottom there is a place where you can leave your review and rating of max 5 points. You user can send only one review. 

::-On the very bottom there is a link to API page. Clicking API button you will generate and will be redirected to a json file with all data from my application.

::-Clicking Log out button session is cleared and users is logging out , login.html page is loaded after.

  
