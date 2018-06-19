[Timeline](index.md) | [Technical Proficiency](technical.md) | [Professional Proficiency](professional.md) | [CV](cv.md)

# TimeLine

## 26/03/18 (Week 1)

Got put in the Semester Tracker project, spent the week Storming and norming, getting to know the other members of the project.  This week we figured out who was going to focus on what part of the project and started brainstorming approaches and frameworks we could use to make the project.

## 02/04/18 (Week 2)

We decided we were going to write the Semester tracker in PHP because our client Elise had already made an attempt at making it.  We used this week to have a look at the yii framework and build a basic project in it to see most of the fundamentals of it.  We also set up a meeting with Adon to talk about what he wants from this software.

## 09/04/18 (Week 3)

We met up with Adon and he told us want he wanted an api to share the database with other projects and to talk to Elise about anything she wanted.  We made the final decision to go with yii framework, built a basic template yii project and spent some time trying to host it locally.  Used this week to look at more advanced yii tutorials and got to know way around basic template file layout, config and database.

## 23/04/18 (Holiday)

Not much was done over this week and last as it has been the holidays, I was sick for a lot of it so couldn't put much work into the project.

## 30/04/18 (Week 4)

Finally got the yii site hosted on WAMP at home and spent bit trying to host it on MAMP on the polytech computers.  I then taught the rest of the group the basics of how Yii works, where to find the main files that might need edited in the folder tree.  I also showed them how to setup the database and host it locally so they could see the changes they had made when editing the files.

## 07/05/18 (Week 5)

The database has now been created so everyone started to work on pieces of the project, my job was to get the data from the database and display it on the website.  I spent this week looking into Gii and how I could use it to create models and views which was pretty simple once I knew what I was doing.  I also got the homepage to generate the current day and week of the semester.

## 14/05/18 (Week 6)

This week I attempted to get a dropdown that would allow for different semesters to be chosen to view.  This required me to do a lot of research on how yii handles forms, I also had a lot of trouble with getting the controller to send the view the information it needed.  Ended up needing a new semester object to passed through and use the yii dropdown handler to display information(semester name) from the database.

## 21/05/18 (Week 7)

I spent this week cleaning up the view I created to show the semester information, originally all logic was thrown into the view but I needed to move this into the controller.  So I had to do some research on how the controller interacts with the view in yii and the syntax needed for what I wanted to accomplish.
Over the course of this week I got assignments showing up next to the weeks they were assigned and holidays showing up next to the week they happen in.  The ability to add data to the database like semesters and assignments was add to the functionality of the site.

## 28/05/18 (Week 8)

This week we got the login system working by checking the database for a created user, also fixed a lot of bugs like multiple assignments on same week messing up table and unneeded tabs in navbar.  A lot of this week was spent working on this portfolio.


## 04/06/18 (Week 9)

This week I worked on getting a working api for use by the learning analytics project or use if this software is used in Project to allow the software to be integrated with other softwares.  My api currently only provides all data from the database in json, I coded a create method for the api too but haven't included it yet as I am unsure if it will be needed.

## 11/06/18 (Week 10)

Showed Adon the api that I had created which currently pulls all data out of the database, he wants me to work on a variation where you can search via url api/<course code> and recieve name, email and username from database for all students in that course.  This requires the database to have a new field added to Course table.
  
## 18/06/18 (Week 11)

Database got refactored with new tables and new fields put in existing tables, I changed the semester view table to now show each day of the week, monday through friday and output if there is an assignment issued, due or a public holiday.  We also created a technical report as a group to hand over to the next team to continue work on this software.
