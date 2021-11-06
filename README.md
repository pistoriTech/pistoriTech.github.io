## Hosting a markdown formatted resume using Github pages and Jekyll



#### Purpose

This readme aims to provide you with the step by step process of hosting your markdown formatted resume on GitHub pages, as well as to discuss the general principles of Andrew Etter’s book [Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) that relate to these steps.



#### Prerequisites

This readme will assume you already have a markdown formatted resume (NEED markdown tutorial), as well as access to a [github](https://github.com/) account that you wish to use to host that resume.



Before continuing to the process of creating and hosting your site, the following is a discussion of the some of the steps you have ideally already taken in preperation for following this readme:

* Firstly, the decision to host your resume online. This is key to one of Etter's basic topics for technical documentation. Hosting on a website allows the material to be corrected and updated almost instantly, and keeps the content as viewed by prospective employers in sync with these changes.  Given that a resume must be accurate and ever evolving, this approach is a perfect fit for this type of documentation.

  While GitHub version control is likely, as Etter describes, "overkill" for non-software based work, having easy access to multiple independent version of your resume is important given different versions may be more appropriate for different employers.

  

* Next, It is important to remember that the benefits of hosting your resume online will be minimal if your resume itself has not been well made. Etter's principles relate even to this preliminary stage of your technical documentation. When preparing your resume remember that, even in a resume, you are writing for an audience.

  Furthermore, Etter mentions the importance of consistency. While this is more easily noticed and corrected in shorter works such as resumes, it is still important to be consistent to avoid confusing the reader with small ambiguities like capitalization and abbreviation use.



* The last point concerning the prerequisites for this readme is the use of markdown for formatting your resume. Here, Etter's principles can be applied more directly. Formatting your resume using a lightweight markup language, in this case markdown, allows you to gain the benefits of easy website creation without needing to use character dense languages like DocBook, which are significantly less human-readable compared to markdown.

  

#### Instructions

While this readme assumes that you already have your resume and GitHub account ready, there are still some steps that need to be taken before those prerequisites will be used.


<br/>
##### 1) Install Jekyll

First, install Jekyll by following [this](https://www.youtube.com/watch?v=LfP7Y9Ja6Qc&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=4) step by step tutorial for Windows installation with two changes. First, when installing ruby follow the suggestions for which version to install given by ruby on the right side of the download page. Second, when you are viewing the RubyInstaller2 terminal and are told to perform actions labeled 1, 2, and 3, you must perform action 2 (MSYS2 system update) last.



Jekyll is a static site generator, and will be used to handwave the more technical aspects of website creation. This allows you to focus on the content you will be hosting. Static sites have a number of additional benefits, even over those from hosting a website in general as discussed previously.



The primary benefits that Etter describes which relate to the hosting of your markdown resume are portability, and little to no installation. The nature of static websites as a series of files makes moving the location of all website related content as simple as any other folder transfer. This also means changing which files are hosted on a site like Githib pages is similarly easy.



The ease of installation, also means that hosting a website locally, such as for testing purposes, takes minimal work. With GitHub Pages this benefit will likely become a necessity, as without the ability to host locally, it can take up to 20 minutes for changes to be reflected in the website.


<br/>
##### 2) Create a static site

Once Jekyll is installed, begin creation the static site. To do this, follow this short and clean [tutorial](https://www.youtube.com/watch?v=pxua_1vyFck&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=4). **However,** there are some changes to these instructions. When asked to perform the command “bundle exec jekyll serve” you must first enter and execute this command “bundle add webrick”, after which you can continue to follow the instructions.


<br/>
##### 3) Add your resume to the site 

Now that you have your Jekyll site created, to put your resume into the site simply navigate to the _posts folder which can be found in the folder created by jekyll, and edit the contents of the markdown file found within such that your resume is below the second set of “---” which is used to contain the title and other information about the page you will be turning into your resume.


<br/>
##### 4) Hosting your resume site

Lastly you will need to host your resume website onto GitHub Pages. To do this you will first need to create a personal access token for your GitHub if you have not done so already. First, sign into GitHub and follow the first 9 of 10 steps as laid out [here](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token). **NOTE:** During step 8, if you are unsure which permissions you will need, select all of them.

Once you have your personal access token, which will allow you to follow along with the git commands for hosting your resume to GitHub Pages, follow along with the instructions in the tutorial linked [here](https://www.youtube.com/watch?v=fqFjuX4VZmU&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=19).

---

You should now be able to view your GitHub Pages site, the link to which can be found under the settings for the repository you created when hosting the site, under the GitHub Pages heading. It will likely be of the form username.github.io/siteName where username is your GitHub username, and site name is the name of the repository you posted the site to. ![ExampleGif](https://github.com/pistoriTech/pistoriTech.github.io/blob/gh-pages/EndProduct.gif)





#### More Resources

[Markdown tutorial](https://www.markdowntutorial.com/)

[Modern Technical Writing by Etter](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)

[Ruby download](https://rubyinstaller.org/downloads/)



#### Authors and Acknowledgements

[Minima Theme](https://github.com/jekyll/minima): Provided by Jekyll along with 65 other contributers 

Group members: Tim Appleyard, Gurtej Boparai, Nelson Yucong Nie, Jordan Unger

#### FAQs:
* Q: Why is Markdown bettern than a word processor?
  A: Markdown allows bare minimum formating and simple style changes, while still making the raw files human-readable in most basic text-editors.
  
* Q: Why can't I log into GitHub on the terminal?
  A: GitHub login on the terminal requires a personal access token ([as described here](https://www.youtube.com/watch?v=fqFjuX4VZmU&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB&index=19)) instead of your GitHub password.
