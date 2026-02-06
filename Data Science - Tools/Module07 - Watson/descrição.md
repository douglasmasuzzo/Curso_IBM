# **CURSO : DATA SCIENCE FOUNDATIONS - DATA SCIENCE TOOLS** #

## Topic : What is IBM Watson Studio ##
 Every business wants to work smarter, and to do that you need to tap into your company's greatest resource, your data. But extracting the full value out of your data isn't always an easy process. First. you end up juggling an incredibly large and complex collection of tools that are used for finding and cleaning data, analyzing and generating visualizations of that data, and using the data to build and deploy machine learning models. And to make matters worse these tools are often a time drain to individually manage, and can be difficult to integrate into your system, which can really slow down the workflow.
 But not anymore. Using Watson Studio you can simplify your data projects with a streamlined process, that allows you to extract value and insights from your data to help your business get smarter, faster. It delivers an easy-to-use collaborative data science and machine learning environment for building and training models, preparing and analyzing data, and sharing insights, all in one place. Watson Studios easy to create visualizations and drag-and-drop code put the power of database decision-making into the hands of any member of your organization with no need for IT assistance. 
 And if you need access to open source tools, the environment offers some of the most popular and powerful ones available. Watson Studio single environment also creates a workflow that's incredibly efficient so data scientists can share assets and work to solve problems within the system rather than starting from scratch every time a new issue arises. And developers can use that efficiency to quickly dive into building machine learning and deep learning algorithms.
 In fact, in the area of deep learning, Watson Studio supports some of the most popular frameworks and can deploy that deep learning on to the latest GPUs to help accelerate modeling by making it easier to use. The environments built-in neural network modeler also helps you build models with a simplified graphical interface even if you don't have the dedicated resources to build a model from scratch, Watson's Studio can help you get started with modeling templates for areas such as visual recognition, language classification, and other tools from IBM Watson services.
 Because Watson Studio is seamlessly integrated with the IBM Watson Knowledge Catalog, an intelligent asset discovery tool, you can transform data and models into trusted enterprise resources and collaborate with confidence, without compromising compliance, security or access control. 
 Watson Studio provides many benefits for organizations helping to infuse AI into the business and drive innovation. You can train Watson Studio with embedded AI services including watson visual recognition. You can customize your models and deploy them as APIs or Core ML by using open source tools like Jupyter, Notebook, Anaconda and RStudio. Watson Studio supports most popular code libraries as well as no code visual modeling with neural network modeler for designing neural architectures using the most popular deep learning frameworks.
 In Watson Studio you can interactively discover, cleanse, and transform your data using data refinery. It helps you understand the quality and distribution of your data with built-in charts and statistics, and provides visualized results through interactive dashboards. Watson Studio includes an intuitive drag-and-drop interface that enables a non programmer to speed up the bottle building process by visually selecting, configuring, designing and auto coding neural networks. 
 From development and training to production and evaluation, Watson Studio tracks your models over time to ensure you have the best performance for any given task using the best solutions across the entire lifecycle of your machine learning models.

## Topic : Watson Studio Introduction ##
 Watson Studio is an integrated platform of tools services and data that helps companies accelerate their shift to become data-driven organizations. You can start with a free account to explore its capabilities. Data science is a team sport we have different types of people interested in the insights that data science can provide this includes business analysts data engineers data stewards data scientist and developers. Data needs to be located and cleansed, models have to be created, tested, monitored, and updated. All this requires teamwork.
 For this reason Watson Studio was built as a collaborative platform a community of like-minded people. There is a lot to cover in this introduction and will only scratch the surface. You can find more information on the digital technical engagement site at ibm.com/demos. Once you are logged in you may see the get started welcome screen. You can minimize the screen by clicking on the get started button in the upper right.
 One important item that is easy to miss is the hamburger button in the upper left it gives you direct access to projects, catalogs and services among other things. The gallery is particularly interesting. It is a collection of assets including tutorials, notebooks, data sets, articles and papers from multiple sources. New assets are constantly added. Assets can be searched using filters for type, language, technology, topics and so on the results can be sorted by features or by date.
 Manage gives you quick access to specific areas to manage finally we have integrated support and documentation in the Watson environment. As mentioned earlier the project is the center of the collaboration. It is very simple to create a project. You click create a project in the welcome screen or new project and either create an empty project or one from an existing one. 
 Then you give it a name, possibly add a description and you're ready to go. At the project level we also have a menu of options it starts with the overview where you can see basic information on the project this tab also includes a README section where you can get more details on what the project is about. The next one is assets where you can see the data assets, models, notebooks, and other assets that are part of the project. You can go to add specific assets using the add to project drop down menu at the top of the screen.
 We won't go into all of those menu items but one important one to know is connection. This allows you to access data that comes from outside Watson Studio as you can see it includes a lot of data services from IBM but also quite a few from third parties such as Amazon and Microsoft. Going back to our project I'd like to point out the environment section. One important tool for that exploration, data manipulation, and model creation is the notebook. 
 Depending on the amount of work that needs to be done we have a choice of resource allocationwe can also tailor the environment to include additional libraries so we have a complete environment from the start. I want to point out two more selections from the top menu access control and settings. The access control allows you to control collaborators and their permissions and more. In the settings section you can among other things, add services. For example you click on the add service drop-down menu, select Watson and add a machine-learning service.
 You have the choice to add an existing service you may have created earlier in another project or create a new one. Note that most services include a light free version. This means that you can experiment with all sorts of capabilities for free.

## Topic : Craeting an Account on IBM Watson Studio ##
 This video shows you how to try out IBM Watson for free. IBM Watson gives you access to IBM Watson Studio, IBM Watson Knowledge Catalog, the data refinery, machine and deep learning, visual recognition models, dashboards and streams flows. At https://dataplatform.cloud.ibm.com/ you can sign up for a free trial.
 When you sign up for an IBM Watson account you are automatically signed up for a free IBM Cloud account. Here you see the Watson applications that will be provisioned. IBM Watson Studio and IBM Watson Knowledge Catalog.
 If you already have an IBM cloud account then use your IBM ID to sign up for IBM Watson.Otherwise, type your email address which will be used to create an IBM cloud account for you. On the next screen you are redirected to the IBM cloud registration page where you need to provide the typical basic information for an account then click create account. 
 Now check your email and confirm your account. Now that you've registered for IBM cloud you can use those same credentials to sign-in. Next you'll see the process create the IBM Watson user account using your IBM cloud credentials and finally you'll see that your account was successfully created. This IBM account has only one Associated IBM cloud account and one resource group.
 If you have more than one associated account or one account with multiple resource groups then during the Watson Studio account setup you'll see this screen giving you the option to select an account and resource group to use. IBM Cloud uses resource groups as a way for you to organize your account resources in customizable groupings so that you can quickly assign users access to more than one resource at a time. View the settings to verify the applications and services that are provisioned. Now you're ready to start working in IBM Watson.

## Topic : Jupyter Notebook in Watson Studio ( Parte 1 )
 This video covers the basics for working with Jupyter Notebooks in Watson Studio. Start in a Watson Studio project and add to the project a Notebook. Just provide a name in a description and create the Notebook. Let's first load a file so you have some data to work with. From the files slide-out panel browse to select the file. After the file is added to the project its available to work with in this Notebook, just click insert to code and insert a panda's data frame.
 Before running the Notebook it's a best practice to insert a cell at the top to describe what the Notebook does. Change the cell type to markdown so this cell
 will not be treated as code and then add the description. Now you're ready to run the Notebook. The inserted code loads the data set into a data frame using your credentials for your cloud object storage instance and then displays the first five rows of the data set. Before returning to the project save the notebook.
 On the assets tab you'll find the Notebook. If you open the Notebook it will be in read-only mode, but you can edit the Notebook and make changes. For example, you can access the info panel and change the name of the Notebook and on the environment tab you could change the environment used to run the Notebook as well as stop or restart the runtime environment. If you'd like to share a read-only version of the Notebook you can do that from here. You can select how much of the content you'd like to share and how you want to share the Notebook either through a link or social media.
 If you'd like to schedule the Notebook to run at a different time you can create a job. Just provide a name for the job and select the scheduling options like specifying a date for the job to run and whether you'd like the job run to repeat. After you create and run the job you can see the status on the jobs tab in the project.

## Topic : Jupyter Notebook in Watson Studio ( Parte 2 ) ##
 This video shows you how to create a Jupyter Notebook. Let's start by adding a data asset to the project. You can either browse to select files or drag files into the panel. Great, now the data file is uploaded to object storage and available as a data asset in this project. Next, create a Notebook. Provide a name and a description and then select the runtime to use when running this Notebook. Here you see the environments you could use.
 You'll learn more about environments later so for now just select the default Spark Python environment and verify the language and spark version. When you are ready create the Notebook. Now wait while the runtime environment is instantiated. Once the environment is ready, in the Notebook, access the data sources and locate the file. Click insert to code and choose how you want to insert the data.
 The choices in this drop-down box are dependent upon the language used in this Notebook and the file type. Notice that the inserted code includes the credentials you'll need to read the data file from the object storage instance. When you run the code the first five rows display. Now let's take a closer look at environments on the environments tab
 you can define the hardware size and software configuration for the runtime associated with Watson Studio tools such as notebooks. You can see that there is one active environment runtime namely the runtime being used by the Notebook you just created and here are the other default environments.
 You can view any of the default environments to see a summary of the configuration and also create a new environment definition. First provide a name in a description. If you select Spark for the type you'll see some additional configuration options. In this case just accept the defaults and choose Scala for the software version. When you are ready create the new environment. The environment is ready for you to use with a Notebook. To switch a notebook to use a different environment, you need to first stop the kernal.
 Then you can change the environment and select the custom environment you just created and associate that with the Notebook. Now open the Notebook in edit mode and wait for the new environment to be instantiated. Since this notebook was last saved using a different kernel you need to set the new kernel. Let's delete the existing cell, locate the source data file, and insert a Spark session data frame. When you run the code the first five rows display. Now you're ready to explore the community and find sample Notebooks and data sets to get started analyzing data.

### _Application - Lab_ ##

 - [**Instruções - Conta Clound**](Instructions%20-%20Watson%20Account.pdf)

---------------------------------------------------------------------------------

### _Review Questions_ ###

 1. _Fill in the blank: In Watson Studio, a ~~()~~ is how you organize your resources to achieve a particular goal. Resources can include data, collaborators, and analytic assets like notebooks and models._

    > Resposta : **Project**

 2. _Fill in the blank: It's a best practice to remove or replace ~~()~~ before publishing to GitHub._

    > Resposta : **Creadentials**

 3. _Which of the following do you need to create in order to publish a notebook to your GitHub repository?_

    > Resposta : **Access Token**

 4. _Fill in the blank: If you'd like to schedule a notebook in Watson Studio to run at a different time you can create a(n) ~~()~~_
    
    > Resposta : **Job**

 5. _Fill in the blank: On the environments tab you can define the ~~()~~._

    > Resposta : **Runtime configuration for flow editor**

 6. _Fill in the blank: When sharing a read only version of a notebook, you can choose to share ~~()~~._

    > Resposta : **All content including code**

 7. _Fill in the blank: When working in a Jupyter Notebook, before returning to a project, it's important to ~~()~~._

    > Resposta : **Save your notebook**

 8. _Fill in the blank: Before running a notebook, it's a best practice to ~~()~~ to describe what the notebook does._

    > Resposta : **Insert a cell at the top of the notebook**

 9. _Fill in the blank: In the ~~()~~ tab you can define the hardware size and software configuration for the runtime associated with Watson Studio tools such as notebooks._

    > Resposta : **Environments**

 10. Fill in the blank: IBM Cloud uses ~~()~~ as a way for you to organize your account resources in customizable groupings so that you can quickly assign users access to more than one resource at a time.

    > Resposta : **Resource Groups**
