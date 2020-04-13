# kjogendra65-gmail.com
Quiz Contest
Instruction page
Student enters Roll No. here
Quiz page
Timed-Quiz appears here
Result page
Result of the user is shown here
Login Page
Admin has to login here first.(admin, 12345)
Admin page
All admin related functions are here!
Videos
Users can also watch a video during the quiz. Or anything you want to display to them.
APIs used to enter and Display Programming codes
CodeMirror In-browser code editor.
SyntaxHighlighter JavaScript code syntax highlighter.
Coded & Tested using-
XAMPP for Apache server and MySQL.
Sublime Text for code editing.
Firefox and Chrome browsers.
Mac OSX & Windows.
How to install on your system-
Install XAMPP and make sure Apache Web Server and MySQL Database are running
copy-paste the quiz_system_git folder in htdocs folder associated with XAMPP
goto phpMyAdmin and create a database.
import the quiz database from database folder into it and make sure it has all 5 tables.
Truncate the tables to have clean database.
INSERT first admin in the admins database.
make required changes in scripts/connect_db.php
Get favicons-
visit faviconit (© 2013-2014 Eduardo Russo).
Upload atleast 200x200px img with maximum 1MB size limit.
click on favicon it! and download the zip file.
extract the faviconit.zip in the img folder.
Add videos in webm(video.webmhd.webm) and mp4(video.mp4) formats in videos folder.
login to the admin page using http://localhost/quiz_system_git/login.php
start the quiz @ http://localhost/quiz_system_git/
Features provided for the Admin in admin.php page-
Clicking on your username in the navbar refreshes the page.
Quiz Homepage opens the Instructions page in a new tab.
Manage Questions-
Create a Question-
True/False - Create a Question with 2 options- True and False.
Multiple Choice - Create a Question with 4 options.
View All Questions-
Shows all the questions of all the quizes on a single page along with the correct answers.
Edit a Question-
Select one question from all the questions in all quizes to edit.
Delete Some Questions-
Select as many questions as you want to delete from the database.
Delete All Questions-
Deletes all the questions from all the quizes, but leaves the quizes intact.
Quiz Management-
You will see all your quizes lined up here.
Add New Quiz-
Add a new quiz to the database and allot the Duration for the quiz, and Max no. of Questions to be displayed to the users.
Further list contains QuizName along with the time and no. of questions allotted to it.
####### Hovering over a QuizName-

Quiz Settings
Set Default - Sets the quiz as default i.e. it will be the one USER will be attempting.
Update Metadata - edit the Duration for the quiz, and Max no. of Questions to be displayed.
Delete this Quiz - Deletes the quiz along with all its questions.
Manage Questions
View All Questions - Shows all Questions of the quiz
Edit a Question - Edit a single question from the quiz
Delete Some Questions - Delete some questions from the quiz
Results
Result(Top 20) - Shows the top 20 Rank Holders.
Result(All) - Shows all the users, sorted according to rank.
Clear the Result - Delete all records of the users who took this quiz.
Settings
Register an Admin
Register a new admin
Change Password
Change password to your account
Delete Your Account
Delete Your admin account
Reset All Tables
Truncates all tables and sets one admin ID as default (admin, 12345)
LogOut
Log out of your admin account.
Interface for Creating/Editing a Question
Select/re-select the quiz to which you want to add/transfer the question.
If there are no quizes in the dropdown, create a Quiz first.
Type/Change your Question.
If there's a program/code in the question,
Select/Change Language of the code
Add/Edit the code below
If adding a True/False Question-
Select the correct answer
If adding a Multiple Choice Question-
Write/Edit the 4 options(single lined) and choose the correct one.
Click Add to quiz/Save.
Interface for Viewing/SelectingForEdit/DeletingSome Questions
Quiz_Name is displayed above its question.
If there's code, it'll be displayed after the text part of the Question.
Options are displayed below.
Correct answer is Underlined and Emphasised!
You can select only 1 question for editing.
You can select any number of questions to delete.
Result Interface
List is already sorted according to their ranks.
Ranks are decided on the basis of highest marks first, followed by the time taken by the user to finish the quiz.
TimeStamp contains the time user started the quiz.
Features provided in other pages
# index.php(Instructions page)
Quiz name along with no. of questions to display and durations is displayed here.
An overlay is provided, currently used to display a video to the user while they wait to start the quiz.
User can't proceed without entering the username/RollNo.
User can't attempt the same quiz twice.
HTML can be edited to add your own rules and the like.
Right-click is disabled.
# quiz.php(Quiz page)
Quiz name is displayed on the top
Countdown is fixed & displayed on the top-right of the screen.
At zero the quiz will automatically be submitted.4.
There's no negative marking.
User can answer none, some or all the questions.
Code/Program will be displayed in color-coded format.
A confirmation dialog will pop-up if the user tries to close, refresh or navigate away from this page.
Right-click is disabled.
An overlay is provided, currently used to display a video to the user during the quiz.
User can't directly access this page.
# result.php(Result page)
Marks of the user are dosplayed here(1 mark per correct answer).
An overlay is provided, currently used to display a message to the user on click.
User can't directly access this page.
if user clicks on back and goes back to the quiz, he can't resubmit the quiz.
# login.php(Admin-Login page)
A user can login from multiple systems at the same time.
User can't access admin page before logging in.
Using sessions to store the session of an admin. Re-login isn't necessary as long as the admin doesn't click logOut.
Miscellaneous features
Using codemirror to have a better textarea input for programs/codes.
Using syntax highlighter to display the code better in a question.
A lot of MYSQL error checks are in place in case of some unknown error.
Basic failsafes are in place for things like SQL injection.
Layout is designed keeping different window sizes in mind.
It isn't designed to work on Internet Explorer also. So, it might be displayed differently on that(Styling difference).
None of the other pages can be accessed directly except the logout.php as it can only be accessed by the admin to logout.
© 2020 GitHub, Inc.
