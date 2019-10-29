# How to Host Your Resume on GitHub Pages

## Who Is This For?
This README is written for newcomers to all of the technologies used in this set of instructions. If you haven't used or even heard of Markdown, Github, Jekyll, or Atom, no problem! I will guide you through the necessary steps to learn how to write Markdown using Atom, and host your own resume on Github Pages with the help of Jekyll. This guide is accompanied by the use of GIFs throughout to show you, visually, where everything is and how its done (finding your way in new programs can be confusing!). 

## Prerequisites
1. A free Github account ([Click here to create a new Github account](https://github.com/join)).
2. Atom, free text editing software ([Download can be found here](https://atom.io)).
    * You will need to add the [Markdown Preview](https://atom.io/packages/markdown-preview) extension as well. 
    * You should be able to add this extension easily by clicking the 'Install' button on the website provided.
        * ![Adding the Markdown Preview extension](https://i.imgur.com/Q3aDeg8.gif)

## Instructions
Once you have all the prerequisites created and/or downloaded/installed, we are ready to start by first creating our Markdown resume!

#### Using Atom to Create Your Resume in Markdown
1. Open up Atom, and create a new file by going File -> New File...
    * ![Creating a new file](https://i.imgur.com/8Y7WO9Z.png)

2. Press and hold <kbd>CTRL</kbd>+<kbd>SHIFT</kbd>+<kbd>M</kbd> to open the Markdown preview beside your newly created file. You are now ready to write your resume in Markdown! I highly recommend following [this Markdown tutorial](https://guides.github.com/features/mastering-markdown/) to understand the syntax provided by Markdown (it won't take long to start writing). 
    * ![Writing Markdown with Preview](https://i.imgur.com/aKgcKoK.gif)

3. Once you are finished writing your resume, you will want to save a copy of your resume (we will not need the file itself, but just in case). Go to File -> Save File As and name your file, ensuring that the file extension is '.md' for the correct format. 
    * ![Save your Markdown resume](https://i.imgur.com/w8eqLlU.png)

#### Creating the Repository in GitHub
4. Log into GitHub by clicking the following link: [GitHub login](https://github.com/login).

5. Click the 'New Repo' button on the left sidebar once you have logged in.
    * ![Creating a New GitHub repository](https://i.imgur.com/rCsKaoj.gif)

6. Create a new repository with the following name format: 'username'.github.io (You will need to replace the 'username' text here with your own GitHub username). This is an important step as this allows us to host a page on GitHub Pages! If you are unsure of your own username, you can see it under the Owner field right beside the Repository name input field (in my case, my username would be brstothers).
    * ![Titling the GitHub Repository](https://i.imgur.com/rOhpKzl.gif)

#### Selecting a Jekyll Theme for GitHub Pages
7. After you have created the repo, you should be sitting on an empty repository page with instructions on how to add files being shown. We want to ignore those instructions and instead head to our repository's settings page to choose a theme for our GitHub Pages website.
    * ![Going to the Repository settings](https://i.imgur.com/0Oetmsv.jpg)

8. Choose your desired theme from the options available. 
    * ![Choosing a GitHub Pages theme](https://i.imgur.com/wGOnTcV.gif)

9. After choosing a theme, the page will direct you to commit an example page featuring the use of Markdown. For now, we will leave the template as is. Title the commit anything you'd like, and proceed to commit the change.
    * ![Committing your theme](https://i.imgur.com/fgiH0lr.gif)

10. At this point, our GitHub Page will be up and running! It can be viewed (although it may take some time to update/show up) by visiting the URL we used to name our repository. That name being, 'username'.github.io (again, we need to replace the 'username' text with your own username, e.g., my own page would be viewable at brstothers.github.io). Currently, there should be two files inside of our repository: _config.yml and index.md. The index file is where our Markdown resume will go.  

#### Adding Our Resume to Github Pages
11. We need to edit our index.md file as mentioned in the previous step. Go to the repository's root directory, click on index.md, and then click on the Edit icon to the right of the screen. 
    * ![Editing index.md](https://i.imgur.com/NqrJx8A.gif)

12. Replace the default text content inside of index.md with your resume (you can do this by simply copy and pasting your resume from Atom into Github's text editor). Before we commit our resume, we should add a front matter block to our index.md as well.

13. Copy the below example front matter block given and replace it with your own text. NOTE: The front matter block should be at the top of the index.md file. 
    * ![Front matter](https://i.imgur.com/7tpsx19.gif)

What is the the front matter block? It is used to set variables that allow for more customization,such as setting the title of a website. Here is an example of what a front block looks like:

```
---
    layout: default
    title: Brendan Stother's Resume
    header: Brendan Stothers
---
```

What do each of those variables mean in context? I'll explain using the above front matter block as given.
* Layout, this selects which layout file Jekyll uses (we don't need to know the deeper details, only that default works perfect for this purpose).

* Title, sets the title of the website that appears in the tab.
    * ![Title text](https://i.imgur.com/oypcHK4.png)

* Header, this text will appear in the top banner of our resume on Github Pages.
    * ![Header text](https://i.imgur.com/H6RMU94.png)

NOTE: If you want more information about front matter blocks, check out [this Jekyll documentation page](https://jekyllrb.com/docs/front-matter/).

14. Commit the changes you made to your index.md file (the changes being: the addition of your resume, and the addition of a front matter).
    * ![Committing your resume and header text](https://i.imgur.com/Jw1dis3.gif)

15. You are done! Your resume should be viewable at username.github.io. At this point, you can easily change the theme without the resume text itself being affected (following the same steps as above).

## More Resources
* [Github Markdown Guide](https://guides.github.com/features/mastering-markdown/)
* [Markdown Cheatsheet by Adam Pritchard](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
* [Jekyll Front Matter Documentation](https://jekyllrb.com/docs/front-matter/)

## Authors and Acknowledgments
I want to thank both David Penner and Proyash Saha for reviewing and editing this README for clarity. I also want to thank GitHub for providing a number of default themes (I used the Cayman theme) for GitHub Pages.

## FAQs
Why isn't my resume showing up at username.github.io?

* This could be due to a few things. If you just updated your resume and aren't seeing the update immediately, give it 10 minutes to update (may take awhile to see the changes). Ensure that index.md is named correctly, as the GitHub Pages layout will look for that specific filename. 

What if I don't like any of the default Jekyll themes provided by GitHub?

* There exists multiple sites that provide a whole variety of different Jekyll themes. Just by googling 'github pages jekyll themes', you will be able to see plenty of different layouts ([e.g., JekyllThemes](https://jekyllthemes.io/github-pages-themes)). However, that is beyond the scope of this instruction set, and you'll be on your own with that pursuit.
