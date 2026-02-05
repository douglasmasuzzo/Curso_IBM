# **CURSO : DATA SCIENCE FOUNDATIONS - DATA SCIENCE TOOLS** #

##  Topic : What is RStudio IDE? ##
 Well now let's have a look at RStudio. RStudio is a IDE, an Integrated Development Environment. It's made for the programming language R. R is a statistical programming language which has been derived from the closed source S language. So R is open source, RStudio is open source and it is completely for free.
 The central data structure in R is a data frame, so we have here a window which contains an editor and below we have here a window which contains a console. So the R interpreter is the interactive interpreter, so you have access to the interpreter here at any time, but its handy if you have a text editor here. You can always execute the code you're writing here in this text editor. On the top right you have another window where your environment is displayed so every variable on the heap is accessible and you can also inspect it. And if you plot graphs, they are ending up here.
 So lets start with data frame. So in order to find out where we are, we say, 'getwd' (which stands for) working directory. So we are in the home folder That's pretty cool, so now we say 'data frame='. You might have seen this symbol here , that’s only a slight difference in function calls. Don’t worry about it unless you are using it in function calls.
 So you can use the normal ordinary assignment operator which makes ours look a bit less ugly. So we say now 'read.csv' and now we can say, go to my downloads folder, and in here we see all the possible files. So I know it started with c-u so its customer messages. And with alt + enter we can execute this line, and then this line gets copied to the console and then gets executed.
 So at the same time you see here data frame is basically containing the data from the csv and you can now have a look at the contents of the data frame if you say view and d-f. And you see here it's already shown inside the editor window. What we notice is, that the first line has been interpreted as header, that’s something we don’t want. So we can say 'header = FALSE'. It's very handy that you have all the completion here, you always know what parameters a function has.
 If you now have a look at data frame again, you see here the first line is now apart of the data and not the header. So, that’s how you can load data. You can of course also load data from remote data base systems, you can use ODBC format
 but that’s beyond the scope of this tutorial. What I want to show you is another way of importing data. 
 You can say here, import from csv and then the code is actually created for you. So lets open the file again, basically doing the same just that you have an idea. You have a data preview with the same problem that you have the first line interpreted as header. 
 So you can actually uncheck this one here and then it's as it should be. And then you say import you notice here you have a second object here on the *heap*, which is called customer messages it's also data frame and it's also shown here.
 So that concludes the first video. In the next video I will show you how to work with libraries, and then after that I will show you how to create plots.

## Topic : Instaling Packages and Loading Libraries in RStudio ##
 One of the main strengths of R is not very nice looking syntax of course, it’s the abundance of packages. So if you go to cran.r-project.org, this is The Comprehensive R Archive Network. You have a link here for packages and you see here table of available packages. You can also sort by date or name, so you get around 15,349 packages.
 And that’s a lot so I’m audio guy. So lets have a look over here for audio.
 So there’s and audio package. If you want to install such a package in R, its pretty straightforward. What you need to do is you say, ‘install.packages’ and then you say the name of the package, ‘audio’ and then you just execute. It asks me whether I want to compile it from source, this is fine.
 So a lot of the R packages are written C or C++ so you need to have a C compiler installed, and then the package is compiled on your machine for you. So this is done, in order to use the package you need to load it. Say library or you can also say require, it doesn’t matter and then you say audio. So now the package is loaded and you see that also here, that the audio package is now loaded.
 And now you can use it. So, if you want to have a look at the source code or some examples, you can just drill down from the R archive. So I’m going here to this URL, and you see here it’s a little example. So this should play a sine wave, lets actually have a look whether I can connect to my microphone with my speaker.
 If that works, ok can you hear that? Ok so that is an example how easy it is to install and use packages in R. And the problem is not that you wont find a package for a specific task, the problem is more that you have five or ten different packages for a specific task. And you need to read a lot and decide which one you are using. So in the next video I will, how to plot in R studio usning ggplot.

## Topic : Plotting within RStudio IDE ##
 So, before we can plot something which just need to have a little bit of data that's very easy to create. That is a rnorm function which samples from a normal distribution. So by default we have mean zero and standard deviation one so let's sample hundred points here.
 And let's do the same for y. and actually increase the standard deviation a bit. And now we create a data frame and it’s data.frame and you say just (x,y). If you now view this data frame we see here that you have the two columns. And you see here the numbers are a bit higher because the standard deviation is higher
 And now we can plot it. So we have to import a library (ggplot2). And then we can actually plot it so we say ggplot plus parameters of course the data frame And I won't go into detail here because ggplot is relatively complex but a very, very powerful library.
 We are basically saying here that we want to draw points. So you see here that on the x-axis and the y-axis we are just plotting those points. Okay, now let's actually plot something more nicely. So there is a data frame build into R which is called mtcars. And it has different types of cars, and their properties.
 So it's a nice data set to play with. And as I said ggplot2 is relatively complex so I'm just copy-pasting the code for plotting something really nicely. So this is basically the weight of the car over the mileage. And you see here the more heavy the car gets, the less is the mileage. And in addition to that you are also drawing a regression line and also a confidence interval or a standard deviation.
 So that's pretty cool with only two lines of code You can create plots which you find in the best (scientific) publications because the best publishers often use R and ggplot2 for creating that plot. Okay, I hope this helps. If you have any further questions, please let me know in the Comments section below. And have a nice day. Bye!


### _Review Questions_ ###
 
 1. _Which of the following functions does RStudio unify? (Select all that apply.)_

    > Resposta : **Editing and execution of source code | Display of the R console | Visualization of plots | Visualization of data in table from** 

 2. _Which statement is true about the RStudio IDE?_

    > Resposta : **RStudio is free and open source**

 3. _Which statement about R packages is correct?_

    > Respsota : **R currently supports more than 15,000 packages which can be installed to extend R's functionality.**