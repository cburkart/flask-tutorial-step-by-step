Welcome to a new video of our "Web Development with Flask" tutorial.

In this video we're going to focus on the set up of the application. We will create a virtual environment and install the Flask dependencies; everything that we need to get our application running. 

I want to focus on the running applications so you can try things by yourself and you don't have to wait for the following videos, in which of course we will explain what is going on and how the application actually works. So, let's get started.

As you guys know, all the content of this tutorial is going to be free and open source; you can access all of it on GitHub.

In this case I have created a Cloud9 workspace so you can have access to all the work that we do in after the videos are done.

What we have to do, the first thing we have to do, is create a virtual environment to install a flask dependencies. 

I'm going to do `mkvirtualenv`, the command to create a virtual environment, and I will decide a name that I'd like; in this case I'm just going to use `flask-introduction`. 

Once the `virtualenv` is created you will see that it is active because you will see that flask-introduction that I gave at the start of my prompt.

I will now install the Flask dependencies. 

You will see that these repository also contains a requirements file that basically lists all the requirements for this particular application.

If you, instead of installing Flask directy, want to use the requirements file, you can just use a command like `pip install -r requirements.txt`

It's going to be similar--the good thing about the requirements file is that we can list the particular versions we want to install from the library.

Now that we have Flask installed we need to run our application. 

The main file of this repository is going to be the `run_app` file, all right? You can find it you inside of the 'flask-introduction' directory. Down there you see run `application.py`

I will just do--with my virtual environment active--I will just do `python` ... `.py`

After I do this you guys will see that the console is taken over by Flask--by the Flask server--and you will see soon information messages showing that the application is running. 

After the application is running I can just go to a particular URL...and open it...and I will see that the application is actually going open. 

If I open the library and I see that first application that have I see this "Welcome to our library" message: that is the same one but I'm seeing right here.

Again, I don't want to focus on the details, and in terms of this particular application I just want you guys to have it running.

Every time you access this resource you will get a new log file--or a log *line*, sorry, in here.

There are a few things interesting down here after we import our application, we are setting the debug mode to true and we are making some configurations so it can run smoothly on different platforms.

You might have different issues and you will have to try different configurations for this particular app, but in general terms it's going to be simple to have it running just with these default settings.

Join us in the following video to understand how Flask applications work and create your own website.
