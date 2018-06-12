[Timeline](index.md) | [Technical Proficiency](technical.md) | [Professional Proficiency](professional.md) | [CV](cv.md)

# Technical Proficiency

## Learned a new framework 'Yii'
At the beginning of the project we were prompted by our client(Elise) to considering going with Yii as a framework for our software instead of coding it in straight php like the original files we were given from Elise, who had already had an attempt at making a semester tracker.  I spent a couple of weeks delving into Yii beginning by creating my first website powered by the Yii framework using a basic template found on their site, after doing that I spent the rest of the week looking through all the folders and files in the template models, views, controllers etc.

## Created yii template hosted locally on MAMP/WAMP
To get my Yii project to run I had to run it on a server, I chose to use a local server hosting software WAMP which I downloaded at home.  This was quite confusing at first and I had some trouble connecting to the phpmyadmin database that came with the software, which turned out I needed to configure the db.php file in the config folder of the site to use the username and password it was automatically setup with root/root.  However when I tried to use the project on the polytechnic computers they didn't have WAMP, I found that MAMP was installed on the computers and then had to play around with and learned that software, after configuring the document root the web server was pointing at I was able to run and view the project allowing me to do work at the polytech.

## Learned how to create models(active records) and controllers using the gii module
Once we had a working site and a database setup with tables, I then needed to find a way to get that data and display it on the website.  This turned out to be easily done with a built in module Gii which allowed to you to generate active records for the models in the database which give you easy access the display and change the data.  Gii also allows you generate controllers, forms, modules, extensions and make CRUD to create, read, update and delete data in each model.

* Created a controller to get semesters, assignments and holidays, which is then passed to a view
* Created the view to display semesters, assignments and holidays in a table
* Created a dropdown which allows you to select different semesters
* Coded the landing page to display current day and week in the current semester
* Created an api which access and shows all data in the database in json format
* Codeception
* Learned how to use github pages and jekyll to make this portfolio
