it's 

looking box or flocks Israel in this video we're going to block our first database your web application 

as you guys my munching away Bob without a database is 

pointless 

so what we're going to do is we're going to create a database fit some data to it some initial laid out and they were going to play the beta evening of wedlock 

we're going to show you the process of creating that database plug it in and then fetching the data to create an HTML with containing that data before we go any further I'm going to show you think structure of the database that we will be 

we will continue with the theme huh library and in this case we will have three tables 

book author and country 

the relationship goes his way a book was written by an author and enough for was born in a calm 

so we will have to have references between book and author right who brought to purchase your book and between author unkown 

in which country these offer was for 

the book table past three feels that it has two text fields one of them that title on one of them the ISP in which are seen 

but then it also has a reference to the offer that brought that certain book the reference will be an eighty and it would represent the ID of the author of that brought up for 

something similar is going to happen with it author staple it will have a name author and then we'll have a reference to the country that that's author was born so for example %HESITATION announcer will have a certain name it would have on me 

representing the cow 

three in which in which he or she was 

so now let's see how all of these terms laid to code 

first thing we're going to do is take a look at this key might be having a sequel file you can find in the library schema those 

in this game I you will see that we're creating the three tables so we mentioned before and up below you see 

%HESITATION big simple command that you can run to create a database file I was just go copies command 

and executed in my local 

machine 

do you see it was a file was created down there the library database which in this case represents our entire time 

this is not always from now he's useless into it doesn't have any data 

so what we're going to do is insert some testing data that we have an initial beta dot sequel to populate the database how some a few authors and books to 

so what I'm going to do is just executed similar commands before but in this case instead of passing levers key my I will pass him you shall data dog SQL 

so now let's see how to use these databases to these blame formation in a web 

what do you want to do is take the south first read these authors from the database on this plate and you know what page so I'm going to show you how it will finally look like 

to do so the first thing you have to do is used example own nine simple batteries up in Iran out I'm going to run this application 

I'm of course are going to reload a page to you can see that it actually works 

let's take a look at these particular model 

what we're doing is we're us usual creating a simple flask obligation but ended viewed the hello world view what works a 

where first connecting to a database 

we're using this sequel life three connect 

method from the school life Fremont you'll that is a building modeling the by home language that's why it's so easy to work with sequel light in pipes and that's I told you this set up is going to be 

then we are fed change all that authors from the database with symbols sequel worry we're doing selex ID and name from offer state 

finally we're constructing all is off dictionaries that each picture income paints their ID and the name of the author 

we will then render a template offers up HTML containing the data using the data off the authors we fetch so if I show you that template you will see that we are just showing the information from the first three offers including did I mean ID and the name of that particular office 

we've seen how it's applied a simple database nowhere obligation but if you look closely you'll see that were hard coding the authors of where do you see 

we have already learned how to eat right to release inside our template to display dynamic data forgets about in our next video will keep advancing on her more advanced features of data loaf using databases