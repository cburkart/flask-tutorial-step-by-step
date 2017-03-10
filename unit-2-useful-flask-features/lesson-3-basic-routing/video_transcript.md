it's 

in this video we're going to start getting to more advanced features 

plus framework particularly if we're going to see how to create different routes and how to respond to Dan when there access it by our users or defying climb 

the first thing we have to understand is the concept for our it's basically very different path that our users we will be able to 

a gate 

well obligation 

so for example this is our side the remoter site in his case where are 

seen that particular pa interruption to buy from programming which he's the pot that defines it enter the python course similarly you can access that bands by from programming course with a different path or a different route 

we will be able to define these different routes with flyers so we can respond of course with different contents for 

print rows from the ones who get by doing these was flask is going to be simple we have already defined given routes we don't explicitly saying it by using the opt out the route they crater 

in this case in our heart and our fifth model what we're doing east we are creating to the different functions and they responsive to the prime part 

so the first one forced us keep used to work it's just a simple function that returns are rendered template function 

that is basically a rendering that template our first up HTML so I'm going to pull that out 

I we are going to see here a least of author so we can just run there Indies page 

what we want to do next is defined are sure route that will serve four different authors have for example will have something like out for slash though out for her slash or his out for slash Austin and we want to access to information about all for four dot particular route 

what we see is that it's impossible for us to define all those routes Connie goalie you know python code we need a dynamic way to show an array those frogs 

they way to do that with plus he's by you seen these symbols and you can see it right here and specifying the dynamic 

name that will change with different in this case are 

so every time we both slash cal third slash out first last name we will be getting these particular 

view and the author's last name is going to be binds to the name comes 

so for example 

if I access date Alcor poem out ther slash who what I am doing is basically I am passing the name author last name no skins of the pope so our obligation for example can go to the database unmoved predict how her with the last name pope 

what we're doing in this particular example is different what they're doing is schist 

getting our dictionary with de Gaulle first data indicates that by its last name but %HESITATION it's a simple way to define it without high 

or a bite of database 

right now 

so again we have %HESITATION dynamic deletion rated route which is basically slash out there slash and the last name 

our 

we we can see how we can shed a raid that your elf we could for example just hard coded and this something like slash how her slash both so every time we need to include that part your route we 

Parker 

there is a different number and better way supposed if we ever need to change this particular views 

so we moved to another place 

we should have to go to each one of the places we've included a hard coded view liking these case I would have to manually 

there's a better way and that's a that's going to be performing with that your elves slash form function from the template each 

in this case you will say that you want action rates are your elf for your health for the altar view in this case is the author of you right here and that's the parameters that we including in the Europe for function I do you want to create a URL for Dick I hope for function with the parameter author's last name 

more 

so what we are she rating is basically I'm going to show you 

second 

there you are well 

slash health for slash boards as you can see right here 

the difference is again we are not hard coding the U. R. L. if we ever need to change shape if we are never ever need to change this particular route that your health or function will take care for us 

of all the details 

so let's recap for a second we said we are defining a route we are two Xist hard coding some %HESITATION prepended string in these cases lock out ther slash and then we have a dynamic part that will change depending on their last name cost 

the question now is we are what happens if we could hear announced for that doesn't exist so we are looking disc authors write this author even for and what happens if the author doesn't exist so I'm just going to try that out 

and as you guys will see we have a key error and that of course is expected because the author 

Austin is not created in these pictures how we're schist 

trying to access the outlook without checking if that parking your angst Alpher exists in our diets to 

so what we want to do next is of course do some parking your checks to verify that the information is there and if it's not there we will one 

raise 

some errors and we're going to do it in our next 

uhhuh