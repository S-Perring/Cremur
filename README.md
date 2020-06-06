# Milestone Project 3: Data Centric Development - Code Institute

## Project Purpose
The website and database are designed in response to a real-world problem and with the intention of implementing the 
system for the company I work for. As a plumbing and heating specialist we at Cremur Heating Centre Ltd tackle both 
large scale installs of heating upgrades as well as the servicing and emergency repair of existing plumbing systems. 
While the install section of the business is well served in terms of technology and information systems the service 
element of the business is currently lagging behind. Customer calls are typed on to Microsoft Word documents and printed 
handouts given to the engineers each morning. Information is often missing, and the result is time wasted on phone calls 
and text messages between the engineers on the road and in office administration staff. The purpose of the site is to 
create a bespoke online database which eliminates the need for the paper handouts and centralises the information.
Its main purpose is to be a rolling live call list which is accessible for the in-office administrators and engineers
on the road.

## User Stories
For this project I spoke to the key staff who will be the main users of the system.
### Alice
"As the receptionist and person responsible for booking in the calls I need the system to be simple and easy to populate because
I will be filling in the information while on the phone to the customer."
### Jim
"I'm not very tech savvy so I need it to be as simple and easy to use as possible. I don't need a huge amount of detail about the job
itself but a live list of all the current jobs would be really helpful for all of us involved."
### Declan
"I often find I'm missing Eircode’s or other key pieces of information related to the callout. It would save so much time and energy
if there was one central location where I could find that information as well as any new jobs added to my schedule."

## Functionality
* The website is as simple and easy to use as possible but with further functionality to be added. It features a main page
which is a live call list with basic details about the job and customer contact information as well as the job category and
which engineer the job is assigned to. Callouts can be marked as complete by the engineer on the road and then deleted by the
administration staff when the invoice is raised as there is no need to store this information long term and it could raise
issues with data protection. 
* The page for adding a new callout is designed in a form format to ensure that all essential information is gathered, and the form can be completed by the administrator while on the phone to the customer.
* The search page is still in development and while the current search function is not working it will be completed and 
hooked up at a later stage of development. 

## UX
The website is designed around the concept that simplicity is vitally important. Huge amounts of information are not required, and it is designed to be used both in office and by the engineer on the road on a tablet. The colour scheme is red and grey in line with the company brand and features the company logo. My User Experience Design documentation helped in the original mapping and planning for the project. It is available for review in GitHub through the links below.
* Strategy Plane - [https://github.com/S-Perring/cremur/blob/master/static/Wireframes/Strategy%20Plane%20MS3.pdf]
* Scope Plane - [https://github.com/S-Perring/cremur/blob/master/static/Wireframes/Scope%20Plane%20MS3.pdf]
* Structure Plane - [https://github.com/S-Perring/cremur/blob/master/static/Wireframes/Structure%20Plane%20MS3.pdf]
* Skeleton Plane - [https://github.com/S-Perring/cremur/blob/master/static/Wireframes/Skeleton%20Plane_Wireframe%20MS3.pdf]

## Additional features and project expansion
While the initial basic phase of the project is complete there are a number of areas for improvement and expansion which
will follow at a later date given more development time.
* Improved UX and CSS - Specifically the layout of the call list can be improved as well as the overall look of the site 
as a whole.
* Finish and hook up the search function. While not essential it will aid the in-office administrators.
* Fix the edit task function.
* Add a filter function to the job category and engineer assigned section. 
* Add a facility to take card payments on site in line with the system used by the heating install team.

## Technologies Used
* HTML - For the basic layout
* CSS - For styling and visual appeal
* Python3 - For the functionality
* MongoDB - To store the database information
* Heroku - To deploy the application
* Flask 
* Pymongo
* dnspython
* jQuery
* GitPod
* GutHub
* Materialize

## Deployment and Command Line Usage
The website was created in GitPod and deployed in GitHub pages. The GitHub repository can be found here 
[https://github.com/S-Perring/cremur] 
The deployed site is hosted on Heroku [https://cremur.herokuapp.com/] and will update automatically as 
improvements and updates are pushed to the repository from the GitPod coding platform. 
All coding and initial testing was completed in GitPod. This platform was used to write the HTML, 
CSS and Python3 code. The display and functionality were tested using GitPod and Google developer tools. 
I used the following process to deploy written and tested code to my GitHub repository;
- `git add .`
- `git commit -m "description of update"`
- `git push`
- `git push heroku master`

Flask and PyMongo were installed with the following instructions in the terminal.
- `pip3 install flask`
- `pip3 install dnspython`
- `pip3 install flask-pymongo`

`git remote -v` - was used to check the connection between GitHub and Heroku. 
`pip3 freeze -- local > requirements.txt` - used to create the requirements file. 

## Testing 
The testing was carried out on an ongoing basis using Google developer tools. At the start of the project 
I found it difficult to get the preview function working in GitPod. This resulted in numerous "commits" to
GitHub to be able to see the live version of the site and its current status. 
- Tested the Schedule Call Function - This works but it does crash the system and needs to be fixed.
- Tested the Manage Categories Function - Works well and with no issues.
- Tested the Search Function - Page layout is ok but needs improvements and the search functionality is only partly built.
- Tested the NavBar dropdown - This works well on tablet size devices and mobiles but the layout needs some work. 

## Issues in Development and Ongoing Bugs
### - Issues and Challenges
Development for this project proved to be challenging due to issues with the URI link and initialization of the env.py for security purposes. I also came across numerous issues regarding the versions of Python and Flask I was using. Resolving and eliminating these issues proved to be extremely time consuming and resulted in lost development time but did add greatly to my knowledge in other areas and my understanding of using the command line and importance of the requirements.txt file. 

### - Ongoing Bugs
- When posting a new callout to the database the app crashes. Upon reloading the data has been successfully added to 
the database but this is clearly a bug and one which I have yet been able to identify and fix. This is the first priority
when more time is available to work on the site.
- The 'timepicker' function has been coded out in Base.Html with the intention to fix the crashing it was causing
and facilitate higher quality data being passed through to the database. This functionality is of key importance
to further build on the project. 

## Resources and Code Credits
- The website is based on the 'Task Manager' mini project in code institute but tailored to fit the needs
and requirements of Cremur Heating. 
- Code Institute
- Stackoverflow
- Slack
- CSS Validator
- HTML Validator
- W3Schools
- MongoDB Documentation
- Heroku Documentation
- Google
- WS3 Schools

## Acknowledgements 
Thankyou to Code Institute tutor Miklos and he assistance in helping fix some issues I was having. He was
a fantastic help at a particularly trying time. 

## Final notes and comments
I found the project to be extremely challenging but ultimately rewarding and while the current site is far from a 
polished and finished article there is room for improvement and expansion in many areas. The priorities going 
forward are as follows:
- Fix the issue causing crashing when scheduling a new call.
- Improve the CSS.
- Finish and hook up the search function.
- Fix the "edit task function".
- Add filters to the call log page.
- Fix the "timepicker".

## Author
Steven Perring