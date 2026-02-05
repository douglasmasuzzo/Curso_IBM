# **CURSO : DATA SCIENCE FOUNDATIONS - DATA SCIENCE TOOLS** #

## Topic : Getting Started with Jupyter Notebooks ##
 So if you want to get started with Jupyter Notebooks, the most easy thing you can do is you just use a Jupyter Notebook service by one of the cloud providers. So within IBM it's called IBM Watson Studio. Watson Studio is more, but it has a hosted Jupyter Notebook service.
 And the other alternative is you just use a system called Anaconda. And that comes with Anaconda Navigator. And here you can install and launch different data science tools. And I'll start here with Jupyter Notebooks first, but I will definitely immediately switch to JupyterLab. I will just show you how Jupyter Notebooks looks like.
 Ok see, this is now Jupyter Notebook. Ok, and the key thing in Jupyter Notebooks is that you can mix and match code, visualizations and documentations. So let's actually create a notebook. And there are various languages supported. Most of the interactive languages.  And I will go here for a Python 3 notebook. But there are also so called kernels for Scala, for R, and any other interactive programing language you can imagine.
 So what you can do here is you can write code, ok. So let's start with a simple Python expression and then the cool this is you can immediately evaluate a variable. So there is no need for printing this variable. Of course you can also do that. But the last variable in the code is always evaluated.
 So for example, if you have Y equals 2, and then you say, Y and X. Then, oh, of course I have to run the cell first. So now you see it's ah, 1. And if it's Y, then it's 2. Ok?
 So that's the basics. So let's actually have a look at how to plot things so you can, for example, create an array. We'll just create a numpy array. So X equals numpy dot array, and then we create here, ah ...1, 2, 3, 3, 3, 4, 5, 6, 7, 8, 9, 1, 1, 2, 3, 4, 5.
 Ok, so that's now a numpy array, we have here you see. And also double check here. If you say type, this is ah, of type nd-array. Ok. So numpy is pretty cool, but I won't go into details here. So we will now import a library called Seaborn for plotting.
 To keep it nicely we put all the imports on top. Then we can say, Seaborn distplot, which is basically a histogram. And then you see here a very nice painted histogram. So it uses, as you can see here, matplotlib in the background. But Seaborn actually acts like a layer on top of matplotlib.
 And turns out the very ugly looking matplotlib plots into something very nicely looking, as we are also expecting, for example, from ggplot2, which we have in R. And the last thing I want to mention here is you can also add another cell and turn this into a documentation cell. So I have selected here Markdown.
 Now I can actually... so let's move this up here. Say, ah, this is a title. Ok?
 Then I can add some, this is interesting. And then, this is even more interesting. You see here it automatically increments the number here. So this is pretty cool because you can just mix and match markdown syntax, your favorite programing language, and all the outputs. So that's only a little introduction and I will now directly move into explaining JupyterLab.

## Topic : Getting Started with JupyterLab ##
 So coming back here to the anaconda navigator, we can also launch here , jupyter lab. So this now looks a bit more complicated, but actually it isn’t because what you can see here is also a jupyter notebook. So you can always download such a jupyter notebook and import it into normal jupyter notebooks. Or you can also import it into for example, Watson studio or any other cloud hosted jupyter environment.
 So, they are all compatible and this is also pretty cool and what you can see here is that there are some more windows. So, you see here a little section so this is a file explorer, and then the other thing you see here, you have a number of so call kernel sessions. So, a kernel session is actually more or less attached to a jupyter notebook. So, this means a jupyter notebook is running in the kernel session and the kernel session is executing your actual code.
 So, you see here this jupyter notebook is of course rendered in my web browser and that’s communicating with that remote kernel. And the kernel is encapsulating the runtime environment, in this case, ordinary python interpreter. You can also shut down those and restart those, here you have some preferences and a list of the open tabs. 
 So the things you can now for example, create a new terminal and you see here there is a second tab opening so you can mix and match jupyter notebooks and your terminals. And you can also drag and drop those around. So you can split and lets add another terminal for example, you can also put it here or here. So it’s a nice way to get and overview of your work. 
 So, create a new python notebook here, and then lets put this here. Ok so you have now, two notebooks and two terminals open at the same time and yeah that’s, pretty cool and that’s basically it. So, now lets close all those. I’ve opened here a notebook from my applied AI course on coursera and you can see here we can execute shell command.
 So, whenever you see and exclamation mark you can directly execute shell commands, so lets do it here. So this is called a ‘pip install upgrade’ and some packages here so some of those are already installed, but some are being collected. And that’s some sort of a best practice. I’m always doing at the beginning of each notebook I will have a pip install, which make sure that I’m always on the correct versions of the dependent software packages.
 So you see here the star, star means that the current cell is just actually executed and once the execution finished, you will see a number. And a number is a task ID and that’s a incrementing number. Based on the number you know in which order you have executed the cells. You also see here, that the jupyter notebook is actually running.
 Now its done, so we see here one and what I always do as well is I’m checking on the correct versions installed. So you see here, I’m checking for tensorflow one fourteen and keras 225. And if that’s not the case I’m raising an exception, so don’t worry about the warnings we are officially on tensorflow 2.x. So I need to upgrade this notebook soon anyway. In case you have a long running task and its just not stopping, you can always restart the kernel.
 So lets do this here, and I’m saying often restart the kernel and clear all output because, once the output is gone I’m really seeing that the kernel has been restarted. So you see here, all your output is gone and that means you have actually shut down the python interpreter and created a new python interpreter in the background here. Another thing which maybe is interesting, lets actually, lets create a new notebook. So you have here, your output one.
 You can always say, ‘ collapse all code’ or ‘collapse all output’. And reopen a different cells, that way you can improve visibility of the relevant content. That’s basically it.
 So there are more things to explore, but I think that knowledge, you can survive. And I think I’ve covered around 80% of what’s important. Maybe one final thing, so you export this notebook into various formats and lets try
 the ‘reveal.js’ slides. Open it in Firefox immediately, and you see here that’s now a reveal.js presentation.

## Topic : Jupyter Architecture ##
 So lets introduce the architecture of Jupyter. So on the left hand side you have of course the user, which interacts with a browser and the central component in Jupyter is the notebook server. So the notebook server is loading and storing the jupyter notebook file and sends the html content to the browser.
 Once this html content in the browser is rendered it interacts with the notebook server using websockets. So its a split application the UI runs in the browser using javascript. And the notebook server is responsible for keeping state, and the second thing is, it is communicating with a so called kernel.
 So the kernel is a wrapper, which wraps the execution framework , for example the python interpreter. So one problem you might encounter if you are running heavy load in jupyter or jupyter lab this is all installed on a single machine, either on your laptop on a server machine. Especially for example, if you are using amazon sage maker, you have the jupyter notebooks.
 But, its all restricted to the machine, the EC2 instance you have chosen before. And another disadvantage is of course, if you are not using the machine you still pay for it. And if its not sufficient then you just either need to wait a long time, or its just impossible to run your workload.
 So you see that here illustrated, we have here a single machine and multipe users for example, are running multiple kernels and eventually the main memory is exhausted and it just crashes. So BOOM! And the solution to this is the jupyter enterprise gateway, which IBM created and which IBM also open sourced which also is now part of the official jupyter open source distribution.
 So the idea is here that, you have a proxy and behind the proxy there is a cluster of machines and that proxy decides where to put the individual kernels and the kernels are then running on those machines. To get a bit more into detail, its here I’m using a architecture diagram, of jupyter enterprise gateway . So you have here, the users on your left hand side as usual there are jupyter notebook instances runnign in the browser.
 So that’s a javascript application and it communicates to the server using websockets, then you have jupyter lab and then, the jupyter enterprise gateway kicks in. So in contrast jupyter lab talking to a kernel it talks to the jupyter enterprise gateway, which acts a proxy. So it basically acts like a kernel but in reality it forwards all the calls to a remote kernel, and the remote kernel is running inside a Kubernetes POD.
 So its basically a container and that container by Kubernetes can be scheduled on any cluster member. And the cool thing here is that you can now just start as many kernels as you like, and Kubernetes takes care of distributing them on the cluster. So of course I don’t want to pitch watson studio here, but you can see here that in the background, while this notebook has been loaded kernel has been initiated on a remote Kubernetes cluster member.
 And whatever you execute here now goes through the jupyter enterprise gateway. I’m just showing watson studio here because I don’t have open source installation available which uses the jupyter enterprise gateway. And if you now for example go through this project overview, then watson studio asks the jupyter enterprise gateway about the status of the different containers, which are encapsulating the kernels.
 And you see here, I have one active environment. This is this one here, you see here the hardware configuration and this is actually running somewhere in the IBM container cloud on Kubernetes. That’s pretty cool and just a final thing, I want to show you here is you can specify environments and you can attach environments to notebooks. So you can basically choose on how many CPUs and how much RAM a particular notebook runs.
 That’s particularly handy for example, if you have ETL task for data integration which uses spark, you just use a spark notebook. And if it’s a heavy task you can increase the number of executors. Or you have for example, tensorflow notebook which then takes this data and does some training. Then of course you can also increase the number of CPUs and main memory.
 That’s basically all and I hope you have learned something about jupyter, jupyter notebooks architecture and if you have questions please post them down in the comments section or use the coursera discussion forum. Thanks a lot bye!

--------------------------------------------------------------------

### _Review Questions_ ###

 1. _Which of the following funcions do Jupyter Notebooks unify?_

    > Resposta : **Editing and execution of Source Code | Visualization of Charts | Editing and display of documentation**

 2. _Which statement is true about Jupyter Notebookks?_

    > Resposta : **Jupyter Notebooks are free and open source**

 3. _What is a Jupyter Notebook Kernel?_

    > Resposta : **It is a wrapper running on the Jupyter server encapsulating the programming language interpreter.**

---------------------------------------------------------------------------

### _Application - Jupyter Notebook_ ###

 - [**Teste Inicial**](Notebook_Teste.ipynb)


 - [**Exercicio - Lab**](Exercicio.ipynb)
