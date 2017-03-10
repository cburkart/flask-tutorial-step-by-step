it's 

in this video equipment to see how to respond to particular errors caused by the use 

sometimes I use her will try to access our resource to Bette and dot no longer sees or sometimes aren't the same user my wanna ox is a particular research that she or he can 

actually 

doesn't she doesn't have the right privilege 

so we will want to respond in some way to these actions and return it on error so the user will be informed about the 

in the previous step we saw how to create basin crowd we were creating a route to man ash particular offers we had an index page that listed all the auth first and whenever we click on one of these offers we will we see more information about 

the issue is that these route was generated than Iomega leaked and these outsourced last name has to exist somewhere 

the big question was what happens if we create an author that for example doesn't exist I was just type anything 

we will receive an error Akira because that particular author was being served from these authors even phone 

dictionary and of course if you try to access at each nodding with them would a wrong key it will raise a key error we're going to see in these next step how to fix that so I'm going to 

command 

fifth pick some poll we're going to go to the number six 

racing counts got some errors %HESITATION we are going to see how this thing is supposed to work if we tried to oxes and offered it doesn't exist we wanna race off for over four error right back an HTTP response with the code for %HESITATION fort defiance spec 

the console right here 

we will see 

that that response we get except for over four not found 

how can we do that mine will get to see it in a sick 

basically we have to do the same huddling us before we get to get that out first last name how we have to first check if our particular off if they keep the altar provided by the use herpes press and in the dictionary that we have all our offer 

again usually will try to catch these authors information from a database on the brush is going to be basically the same will check if they offer exorcist and if the author doesn't exist we wishes to raise an error 

the way to raise an error with plus he's by invoking the support function 

with the particular code of error that you won a race so in this case I have imported import function I will schists race off for over four 

I know you have noticed these but these patients you see right here is a 

patient we have created this is not the default not found page 

created by cost 

plus the latest specify particular patients for errors we want a response of for example if we have 

for four or five hundred error we will be able to create a party your page with that 

every major website will have a heart Europe for four or five hundred and rapacious notches down actually page 

I'm going to show you first how is L. how did 

default for four page in class looks like 

this it isn't it called for four page you plus 

I'm going to show you there how I have created artists and four four page I will show you again that it basically works and that is that we will create an error handler for each one of the errors and we wanna %HESITATION huddle right so eight every time a four four ever happens we while we will respawn with these parts your function weakens it pretty much 

whatever we want each year we can for example create %HESITATION logging 

we what we once who love it sue somewhere saying like look someone is trying to access these parking your patient doesn't exist so we can for example keep track of Orton patients to 

have lost 

there are different things we can do I'm basically classical latest create our view as did a regular one we have right here it will let us create of you soon respond to party your errors 

the rest is simple we have already seen it %HESITATION like she will just go to that for four page and it's what we have right here days though known messaged we have here 

I curator for example to 

no way on I could show just reload days and I will see the message no way 

so again class will let let you create party dinner patient with that you will use to respond 

so that errors 

something interesting to see here is that aside from there rendering that template I am also returning a four oh for each 

alright well I am actually returning from these function and this is not the bands but you have to understand by them 

two two CD's is we are returning topple all rights not topple is a particular data structuring that my whole language pewter Noel topples please go to our instruction going on advanced by phone course 

in this case were returning a couple on lost quite the fool will let you return topples to specify aside from the content of the patient you wanna 

turn depart your status coping 

to return 

by default flasks specify here by two hundred so for example if we go to our first index patient right here lost keys as we are not providing a particular status code flask isn't hurting and we are returning 

two hundred successful code 

finally I want to show you know the future of the flask routing mechanism 

I have noticed but we have a special token that we have included before our prime attorney 

this will lead us specify what data type we're expecting these parameter to me on the school hours %HESITATION to be more concise and we will not have 

specify particular error cases so for example right here we're expecting a stream if they use her is passing and interfere we should have to do some error handling on check if they promise opossums if anything's any to share and they're raising their 

that's a pretty common task and what the Bellman so lost late as 

forget about that error checking and he will later this it will do it by ourselves for us 

so what we're going to do first East command this code 

here 

so we will see how flask hills's without having to specify a particular error checking 

then I'm going to say that I am suspect for example I need to share 

and when I tried to access a piece author with a particular stream what I'm going to get he's began this same error page so I haven't included these because 

course I have commented out I can 

the movie completely to show you 

but the cost is taking care four ounce of returning dot particular four oh four era what happens if I remove these 

in this case I will get again 

key error because the up stream that I passing this and 

so again at some 

particular moments we will have to do special error handling and that's fine be 

we were deprived of their boss is 

okay is good 

train but the author doesn't exist and we will that he's involved with the business logic of propagation 

but there are things of cost can take care of myself lake in these case checking the type of the parameters that we are receiving again flask will save us a lot of time in these parts to your issues so we can create web pages Nomar in a more flosser on peak your way 

finally I want to show you a particular example that deals with authentication each 

we have created another view with a different route that simulates and I mean 

in this case even I am trying to access day of main page 

that I have creative with the routes 

it leads right so it's going to be something like author slash boat slash indeed what I am going to receive itself four oh one error message I needs basic goalie and not an unauthorized error message so whenever you're trying to 

%HESITATION keep I use her way from particular resource you can just use the same abort function by specifying the correct status code again we're sure where she's showing you a few examples four four four one there are many different types of errors on what you have to know here is that by using the airport function you can just use 

pretty much any error that you won 

it's important understand that all these errors will be %HESITATION created based on the business Tawfik off your applications so you will be the one to sign in the proper teacher you certain 

as these resources or if 

cannot access 

it's research and in that case raising the error okay so pay attention to their business 

in these last two videos we have combined data routing system with errors how willing to create a more robust and real a real live application in the following be is we're going to start to competing to more advanced features a flask language and start having more control your obligations to you in the next 

mmhm