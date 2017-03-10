it's 

welcome back to our clocks injury in this video we're going to show you how to use a how to work with static files 

static files are bold defines it are not directly related to our flights complication so for example images CSS files shows good piles again any panic file but it's just not related to our patent application 

how 

circuit we're going to see how to include him I'm how classmates peace process easier 

to show you how athletics files work we're going to use an example 

we're going to start from our previous form there one that we use in our previous step and you will see of course it is a pretty ugly form because 

but if you check take code of closely you'll see that it's our books are violated HTML form so what we wanted to use included there CSS file containing the bootstrap code so we can %HESITATION style these particular form 

if I go ahead and I used to example number fourteen 

I'm reload this page you will see 

but we now have the same form but dont but now it looks much much better and that's because we're shows including their bootstraps uses pile up by 

show you the source code we are now including a reference to the posts up CSS file on this case so excited file 

this is all the code we don't care about it on these what mark cities this topic file 

it's just an external file we use for a particular application 

if you check their code of ethics humble fourteenth you'll see that it's just us the same code as before but now where you see 

so again they mush it seems to be in that family if we check the template that only thing that changes from our previous example is that we are shit including these reference to their books about CSS file 

and we're doing so by using that your love for 

lost function 

they describe this function euro for basically takes on endpoint in 

gays did and one 

product and I finally came to create your health for yeah as the name implies too it's just generating for awesome these particular your L. that these kinds of 

now you might wonder why do we need these 

well in a professional obligation diff rocks server will not be 

serving static files 

static files will usually be served by this from age to be severed you 

is maybe a more complex topic any deals on how obligations are usually deployed but basically you will have a robust HEP server like engine ex or a hot 

and behind got it should be server you will have your flask server plus we'll just take care off the application processing the piping code his service thought of policy issues 

shit is shared files Sears has filed emissions files you will want to use the other more robust and usually a foster HDB server so that's why we needed to construct these in your arms he now in a smarter way in this case as we are developing 

we are serving their stockpile from class but when we move our obligations of production we don't want to go changing that your oil you were ill at any given point where we use them so where you seem Chisti Senora form so you are core function and then we can change the settings depending on how we Diplo deploy our application 

by convention flask will build these your elves and in this case where she's using that word siding because we have us tied a directory containing deposit we want included so right here you can put for example all your image his or her chaise files or years he has has files and just put them here on in the vellum and you can choose to serve them with these you're out for 

there are different ways to serve %HESITATION destroyed a policy for action and of course each use case will change but in general by using these techniques of servings target files you will usually be set 

mmhm