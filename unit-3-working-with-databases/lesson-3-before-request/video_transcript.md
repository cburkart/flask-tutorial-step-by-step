it's 

if you look closely out our previous example you might have noticed something changing the code 

they go to eat per se if this saying it works in the same way bush question all the offers from a database but we have a small chain 

we're not connected to the database inside of you anymore but now we have these before request function 

we have days before August function which is basically decorated with it up dog before request undead is that these particular function right here is going to be invoked every time that every new request how 

so let me for example put a print statement here 

and 

invoke the same patient we're looking again 

if we look closely at the logs 

we will see Vera hello world strain we printed out that it was printed so the before request form 

was 

I want you to picture for a second a large application containing many many many functions and many many many views right I users if you are deaf or view homes you 

sales I know many different patients 

if each one of those patients have to connect to the database Biloxi of including that connect database the connections of batteries inside of you could be duplicated 

so wide relying on the before request %HESITATION hook weekend 

connected database she 

glued to coach going through the violations winds and then re use it in every author view 

to do so we make use often sheet of cracked off the flask framework 

to be honest these name is terrible this is my opinion the sheet 

I'm Bob viable name she but it it stands for the global auction 

and it's an option that we can use when we need to invoke different functions to fulfill %HESITATION some certain details for just one request though you have different functions that are collaborating to fulfill a single request 

so the data we wanna persist in the global log shaped is going to be in this case the chronic 

database 

when we've been invoked hello world view 

we will be able to use that database connection bassist invoking she thought the V. as you can see right here 

I means include now another view should sit down if you to demonstrate how before request is 

it included in everything classically Manx inside %HESITATION will by doing that we will see day hello world I string printed in 

so let me clue it is simply being here it's just slush extra I'm going to save this script and then I'm going to invoke extra right 

if you check closely you will see that all other view was executed on we see a right here they him though warm strength so what if this is telling us is that just before requests will be executed before any request so if there is any 

type of work did you have to do before every requests for example checking if there is no use %HESITATION log to use for checking if they log in user has the right privileges eve third is setting up some type of clogging any task that you have to do before every request well that before request kook isn't really really good eighty 

mmhm