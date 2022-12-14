# Creating your own Resume Webpage

![Animation](https://github.com/Luc-Miron/Luc-Miron.github.io/blob/main/2022-10-31%2010.54.44.gif)

### [Demo Website](https://luc-miron.github.io/)

## Purpose

The purpose of this document is to demonstrate the use of the following Web-Based Authoring technologies through the creation of a static resume hosting webpage:
* lightweight markup language (Markdown)
* static site generator (Jekyll)
* distributed version control system (GitHub/GitHub Pages)

This project was inspired by the book [Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS) by Andrew Etter. In this example we will edit a resume in Markdown, use Jekyll to format the static site and provide instructions on using a distributed version control system to host your own resume webpage (GitHub/GitHub Pages). In the following sections, you will see some pre-requisites you will need before getting started, the basic instructions and more resources to keep you going once you have the basic site up and running.

## Pre-requisites

1.	 GitHub account. (You can create one on [GitHub](https://github.com).)

2. 	 Up to date resume written in Markdown. Click [here](https://owl.purdue.edu/owl/job_search_writing/resumes_and_vitas/resume_workshop/index.html) to learn how to write a well formatted resume.

> If you have no idea about GitHub or Markdown and how they are used, I highly suggest starting with the [More Resources](#more-resources) section of this document where you can find material to familiarize yourself with these tools.

## Instructions

### Setting Up The Repository

> In this section, we will create your GitHub repository to host the files for your webpage.

1.  In your GitHub account, go to your '_**profile icon**_' at the top right of the screen and select the drop down.

2.  Select '_**Your repositories**_'. This view shows all the repositories associated with your account.

3.  Inside the repositories page, locate and select the green '**_New_**' button at the top right, just below your profile icon.

4.  Complete the '**_name_**' and '**_description_**' fields for your new repository.  

	> Be sure to name your repository _**Firstname-Lastname.github.io**_.

5.	Select '**_Public_**' for this repository.

6.  Select the box to '**_add a README_**'. This will populate a generic `README.md` file with the name and description of your repository. You can customize this later.

7.  Select a '**_licence_**' from the drop-down box. I use the **GNU General Public Licence** but you can use any you're familiar with. 

8.  Finally click the '**_Create repository_**' button at the bottom and your repository will be generated with the licence file and a README containing the name and description of your repository.

### Importing Your Resume

> In this section, we will import your resume to the GitHub repository and edit the filename to ensure it launches correctly in your webpage.

1.	 From the main branch page select the '**_Add file_**' drop-down and select upload file. This will open the upload window.  

2. 	 Use the drop box feature or select the choose file option inside the box to upload your Markdown resume. The filename will then be in the display window above the comment boxes. 

3. 	 Select '_**Commit changes**_' to add your resume to the repository.

4. 	 Select your resume file in the main branch of your repository.

5. 	 Select the `pencil` icon to edit the file.

6. 	 Rename the file `index.md`. 

7. 	 Toggle between the preview and the edit views at the top left of the document to make any required changes to the document or to fine tune the layout. For Markdown formatting tips, you can refer to this [cheatsheet](https://www.markdownguide.org/cheat-sheet).

8. 	 Commit your changes to the main branch by selecting '_**Commit changes**_' at the bottom of the page.


### Setting a Theme

> In this section we will set up a theme for your resume hosting page using the GitHub Pages supported Jekyll themes and their static site generator.

1.	 Create a new empty file in the main branch of your repository named `_config.yml` using the `Add file` dropdown.
2. 	 Browse the [GitHub Pages supported Themes](https://pages.github.com/themes/) and choose a theme. 
> Look through each README to find out about that particular theme.

3. 	 Copy the code from step 1 of the '_**Usage**_' section of your chosen theme into your `_config.yml` file. It should look something like this:

```
remote_theme: pages-themes/leap-day@v0.2.0
plugins:
- jekyll-remote-theme # add this line to the plugins list if you already have one
```

4. 	 Copy the code from the first block of the '_**Customizing**_' section of your theme's README in your to your `_config.yml` file and edit with your relevant information. Here is an example:

```
title: [The title of your site]
description: [A short description of your site's purpose]
```
5.	 Commit the new `_config.yml` file to the repository by selecting the green **_Commit new_** file button at the bottom of the page.

### Launch

> In this section, we launch your resume hosting site and see the theme in action.

1.	 Select the '_**Settings**_' tab at the top of the page.  
2. 	 Select the '_**Pages**_' subsection under the Code and Automation header in the left vertical menu area.
3. 	 Select the source '_**Deploy from a Branch**_' under the Build and Deployment heading.
4. 	 Set the branch to '**_main_**' and the folder to '**_root_**' under the '_**Branch**_' sub-heading.
5. 	 Check out your rendered resume on your site by selecting the '_**Visit Site**_' link once it has finished being built by the GitHub Pages workflow.
	
>  It may take a few moments for the site to build before the '_**Visit Site**_' link becomes available. Your page will be hosted at https://[Firstname]-[Lastname].github.io/ by default.
	
6. 	 Now, you should work on editing your README to let people visiting your repository know more about it's contents and purpose. Check out this [list](https://github.com/matiassingers/awesome-readme) of READMEs as examples.
> Consider adding a [GIF](https://josephcardillo.medium.com/how-to-add-gifs-to-your-github-readme-89c74da2ce47) like the one at the [beginning](#creating-your-own-resume-webpage) of this document to make your README more appealing or demontrate part of your process.
	
### Summary

Now that you have the basic resume setup and you've begun familiarizing yourself with static site generation on GitHub using supported Jekyll themes, you can explore some more elaborate setups using Markdown, GitHub and Jekyll. Here are a few templates to get you started:

 * 	This is a nice [clean template](https://github.com/sproogen/modern-resume-theme) which is also set up to be hosted on GitHub pages.
 *  This [example](https://github.com/ankitsultana/researcher) uses a welcome page and links to the resume.
 *  This is a nice [basic template](https://github.com/matarjalal/jekyll-resume-template) that can get you started with customizing.
 * This minimal [resume theme](https://github.com/murraco/jekyll-theme-minimal-resume) has lots of room for customizing.

Be sure to check out the [Resources](#more-resources) below to learn more about all the tools we discussed.

## More Resources

1.	 See an overview of Git and GitHub on [Kintsa.com](https://kinsta.com/knowledgebase/what-is-github/).
2. 	 Learn more about [Markdown](https://www.markdownguide.org/getting-started) and practice using this [tutorial](https://www.markdowntutorial.com/).
3. 	 Research some popular Markdown editors at [oberlo.ca](https://www.oberlo.ca/blog/markdown-editors).
4.  Learn more about [YAML](https://docs.ansible.com/ansible/latest/reference_appendices/YAMLSyntax.html) to help customize your `_config.yml` file.
5.	 Learn more about [Jekyll](https://jekyllrb.com/docs/) and static site generation on their documentation page.
6.  Look up [these](https://github.com/topics/jekyll-resume-theme) other custom Jekyll themes. 
7.	 Learn to create a short [GIF](https://josephcardillo.medium.com/how-to-add-gifs-to-your-github-readme-89c74da2ce47) yourself that you can use in your README.
8. 	 Check out Andrew Etter's book [Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS).
9.  Read this [blog](http://elipapa.github.io/blog/why-i-switched-to-markdown-for-my-cv.html) post to find out why this Biomedical engineer switched to Markdown for their Resume.


## Authors and Acknowledgements

* Page and Resume authored by Luc Miron
* Review and testing carried out by Evan Miron
* Concepts and tools from Andrew Etter's book [Modern Technical Writing](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)
* Resume theme ["Leap-Day"](https://github.com/pages-themes/leap-day) by [Matt Graham](https://twitter.com/mattgraham).
* Resume theme ["Dinky"](https://github.com/pages-themes/dinky) by [Parker Moore](https://github.com/parkr), [Filipe Tavares](https://github.com/fptavares) and [Ben Balter](https://github.com/benbalter).


## FAQs

* Why do I see the `visit site` link on the settings page but it's displaying an older version of my resume?  
> Be patient. You have to wait for GitHub to build the updated site. Wait a minute or two, then refresh the page in your browser.

* How do I fix the fact I'm still getting a 404 error even after I waited for the site to build and the link in my GitHub pages menu looks like it's live?
> Confirm all your files are named correctly. The static site builder is looking for specific file names in your repository. Specifically, for the `_config.yml` and `index.md` files. You can also confirm the site is being launched from the main branch and all changes have been committed to main.
 		 	
* Can I edit the webpage so there is a welcome page that links to the resume?  
> 	Absolutely! Check out this [example](https://github.com/ankitsultana/researcher) which is also hosted on GitHub Pages with a welcome page, link to the PDF resume and a contact page. Note how the links and folder hierarchy are laid out. For more information on customizing a your themes check out [Jekyll's documentation](https://jekyllrb.com/docs/themes/).

* How do I change the links in my theme's template?
> Go to the README for your chosen theme and refer to the customization section. You should find instructions on where to change the link information. Often, this is done in the `_config.yml` file.
