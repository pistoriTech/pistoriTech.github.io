## Hosting a markdown formatted resume using Github pages and Jekyll



#### Purpose

This readme aims to provide you with the step by step process of hosting your markdown formatted resume on Github pages, as well as to discuss the general principles of Andrew Etter’s book Modern Technical Writing (https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) that relate to these steps.
  
   
#### Prerequisites

This readme will assume you already have a markdown formatted resume (NEED markdown tutorial), as well as access to a github account (https://github.com/) that you wish to use to host that resume.



Before continuing to the process of creating and hosting your site, the following is a discussion of the some of the steps you have ideally already taken in preperation for following this readme:



* Firstly, the decision to host your resume online. This is key to one of Etter's basic topics for technical documentation. Hosting technical writing on a website has a number of advantages over the older method of distributing pdfs. Websites allows the material to be corrected and updated almost instantly, and keeps the content as viewed by prospective employers in sync with these changes.  Given that a resume must be accurate and ever evolving, this approach is a (perfect) fit for this type of documentation.

  In particular, Etter identifies the importance of recording changes to a product, and of using Distributed Version Control and this is also true of a Resume, which may be adapted to meet the needs of the audience (in this particular case, the persons responsible for hiring into a specific job.)  This Readme describes how to host a resume and changelog on GitHub to facilitate change management, including a log that shows what has been changed.



* Next, It is important to remember that while the benefits of hosting your resume online are many, the benefits will be minimal if your resume itself has not been well made. Etter has guidance that is relevant even to this preliminary stage of your technical documentation. When preparing your resume remember that you are not just creating a isolated list of accomplishments, even in a resume you are writing for an audience.

  While Etter describes three types of audience from the perspective of engaging with a technology, the importance of considering your audience still stands. In this case, while Etter's principles are presented more for documents relating to functional programs and the audience thereof, both the prinicples of audience selection and functional documentation can still be applied to resume writing.

  The idea that documentation should help explain why a reader may care to engage with the product can be contextualized to relate to a resume when considering that, from the perspective of an employer, *you* are the product that is being presented. Further questions that Etter includes under “Basic Functional Documentation” are”How [do you] fit into a broader ecosystem...”. While a resume is not often of a form where engaging in a dialog is appropriate, these points are still certainly considerations for your resume. An additional point brought up by Etter, is the importance of consistency. While this is much more easily noticed and corrected in shorter works such as resumes, it is still a point of comparison between more technology focused of technical writing, and this resume.



* The last point concerning the prerequisites for this readme is the use of markdown for formatting your resume. In this, Etter's principles can be applied more directly. Formatting your resume using a lightweight markup language, in this case markdown, allows you to gain the benefits of easy website creation without needing to use character dense languages like DocBook, which are significantly less human-readable compared to markdown.



Now that the benefits of hosting a markdown formatted resume as well as how that relates to Etter's guidance for technical documents has been covered, next is the step by step guide to implement that desired website.



#### Instructions

While this readme assumes that you already have your resume and github account ready, there are still some steps that need to be taken before those prerequisites will be used.




  
    
##### 1) Install Jekyll

The first step will be to install Jekyll, by following a step by step tutorial for Windows installation with one small change. Once you are viewing the RubyInstaller2 terminal and are told to perform actions labeled 1, 2, and 3, you must perform action 2 (MSYS2 system update) last. With that exception, this ((https://www.youtube.com/watch?v=LfP7Y9Ja6Qc&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=4) tutorial will lead you through the installation.



Jekyll is a static site generator. In other words, Jekyll will be used to (handwave) the more technical aspects of website creation, allowing you to focus simply on the content you will be hosting. Static sites like those built by Jekyll have a number of additional benefits, even over those from hosting a website in general as discussed previously.



The primary benefits that Etter describes which relate to the hosting of your markdown resume are portability, and little to no installation. The nature of static websites as a series of files makes moving the location of all website related content as simple as any other folder transfer. This also means changing which files are hosted on a site like Githib pages is similarly easy.



The relative lack of installation, depending on if you consider a static site generator as part of the installation requirements for the site itself, also means that hosting a website locally, such as for testing purposes, takes minimal work. For this readme this benefit will likely become a necessity as, without the ability to host locally, it can take up to 20 minutes for changes on Github pages to be reflected in the website.




  
    
##### 2) Create a static site

Now that you have Jekyll installed correctly, the creation of the static site is next. For this step as well there exists a very short and clean tutorial that you should follow (https://www.youtube.com/watch?v=pxua_1vyFck&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=4). **However,** with this as well there are some small changes to these instructions. When asked to perform the command “bundle exec jekyll serve” you must first enter and execute this command “bundle add webrick”, after which you can continue to follow instructions.




  
    
##### 3) Add your resume to the site 

Now that you have your Jekyll site created, in order to put your resume into the site simply navigate to the _posts folder which can be found in the folder created by jekyll, and edit the contents of the markdown file found within such that your resume is below the second set of “---” which is used to contain the title and other information about the page you will be turning into your resume.




  
    
##### 4) Hosting your resume site

Lastly you will need to host your resume website onto github pages. To do this you will first need to create a personal access token for your github if you have not done so already. To do so, simply follow the first 9 of 10 steps as laid out by github here (https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token)

Once you have your personal access token, which will allow you to follow along with the git commands for hosting your resume to github pages. To do so, simply follow along with the instructions in the tutorial linked here (https://www.youtube.com/watch?v=fqFjuX4VZmU&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=19).

---

With that done, you should now be able to view your github pages site, the link to which can be found under the settings for the repository you created when hosting the site, under the GitHub Pages heading. It will likely be of the form username.github.io/siteName where username is your github username, and site name is the name of the repository you posted the site to.



#### More Resources

markdown tutorial

link to etters book

at least one other resource





#### Authors and Acknowledgements

template authors?

Group members: 
