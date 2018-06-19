[Timeline](index.md) | [Technical Proficiency](technical.md) | [Professional Proficiency](professional.md) | [CV](cv.md)

# Technical Proficiency

## Getting Elise's original semester tracker to work on the Kate server

When we got put into the semester tracker project Elise gave us the files she had made in a attempt to make her own, I spent a class uploading these to Kate and creating a database which used the same layout she had on phpmyadmin.  I only managed to get the front page working without any css applied to it, we used this in the beginning to get a feel for what the software should look and feel like(links and information shown).

## Composer

At the very beginning I tried to download and get Yii to run on my computer however the YiiFramework site pointed at an application called composer which allowed you to download Yii and extensions such as codeception.  The first roadblock I had was when installing composer you needed to point at a current version of PHP and I couldn't find the location of the php.exe file, it turned out I could find this in the WAMP or MAMP folder.  Once I had installed composer I didn't realise that there is no gui and it is all done from the command prompt and needed to be pointed at globally by adding it to the computers PATH.

## Learned a new framework Yii
At the beginning of the project we were prompted by our client(Elise) to considering going with Yii as a framework for our software instead of coding it in straight php like the original files we were given from Elise, who had already had an attempt at making a semester tracker.  I spent a couple of weeks delving into Yii beginning by creating my first website powered by the Yii framework using a basic template found on their site, after doing that I spent the rest of the week looking through all the folders and files in the template models, views, controllers etc.

## Created Yii template hosted locally on MAMP/WAMP
To get my Yii project to run I had to run it on a server, I chose to use a local server hosting software WAMP which I downloaded at home.  This was quite confusing at first and I had some trouble connecting to the phpmyadmin database that came with the software, which turned out I needed to configure the db.php file in the config folder of the site to use the username and password it was automatically setup with root/root.  However when I tried to use the project on the polytechnic computers they didn't have WAMP, I found that MAMP was installed on the computers and then had to play around with and learned that software, after configuring the document root the web server was pointing at I was able to run and view the project allowing me to do work at the polytech.

## Learned how to create models(active records) and controllers using the gii module
Once we had a working site and a database setup with tables, I then needed to find a way to get that data and display it on the website.  This turned out to be easily done with a built in module Gii which allowed to you to generate active records for the models in the database which give you easy access the display and change the data.  Gii also allows you generate controllers, forms, modules, extensions and make CRUD to create, read, update and delete data in each model.

## Created the view to display semesters in a table

I created a new index view for semester which I generated with gii, I then imported the model for semester into the view and pulled all data out of those tables.  Putting all information into a table and and displaying all week start dates with week numbers, skipping over holiday rows and later in the semester I added assignments or holidays displaying beside the given week they occured in.  I later changed this to display each week and date ranges (monday to friday) and a column for each day, displaying if there is a assignment assigned or due on that day or if there is a holiday.

## Created a controller to get semesters, assignments and holidays, which is then passed to a view

I had written all the logic in the view which led to a lot of code repetition and made it hard to expand on the code and add extra features, so I spent a week looking into generating a controller with Gii and using that to pull all the information I needed out of the database and sorting it the way I needed it.  I then passed all the data and extra variables I had created (like a variable to track which semester we were currently in) into the view, this cleaned up the view and made it a lot more readable.  Later on in the semester we needed to add assignments and holidays so I pulled their data out of the models in the controller and also passed them to the view, because I had cleaned the code this was a very quick and easy process and kept the logic that I added out of the view code.

## Created a dropdown which allows you to select different semesters

Getting a dropdown to allow the user to choose which semester was being displayed took me a while to get working, this was especially hard because Yii uses its own layout for forms which required a model to be passed from the controller and used to create the dropdown with the help of the built in arrayhelper and mapping functions.  The main problem I had with this was that the model needed to be a new empty model of the semester and I was passing it all the data from the semester model, once I had fixed this I pretty much had it all working only needing an extra field in the database table to show what would appear in the dropdown (e.g. Semester 1 - 2018).

* Coded the landing page to display current day and week in the current semester
* Created an api which access and shows all data in the database in json format
* Codeception
* Learned how to use github pages and jekyll to make this portfolio
