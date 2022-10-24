# Publish your Obsidian Notes

I want you to use your own personal memex as a way to share your work online. We are going to set up a semi-automated way to publish _subsets_ of your Obsidian vault. The result will be a website that looks rather like our course website - well, it *should*; I'm using the exact same system!

![](2021-11-22-22-49-26.png)


## Quick start

1. Make a folder inside your Obsidian vault; call it 'website'. Any notes that you create that you want to share on the net will go into this folder for safekeeping (so you can find them easily on your machine.)
2. Create a **new github repository using this template**. Click the green button at the top or use [this link](https://github.com/jobindjohn/obsidian-publish-mkdocs/generate). 

![](2021-11-22-22-54-02.png)

2.  **Give a name** to your repository. By default your notes will be published at `<https://username.github.io/repo-name/>`
     - Copy only the `main` branch while creating the repo from the template (this happens automatically, so you shouldn't have to work about that.)
3. **Newcomer**  Make a new note in your 'website' folder; call it `index`. This will be the 'home' page of the website. 
	1. Find this note on your machine (use Windows Explorer or Mac Finder or right-click on the file name in Obsidian's file list on the left side of your screen and select 'reveal in finder')
	2. In Github, in the repo you just created, click on `docs` in the middle of the screen
	
	![[Screen Shot 2022-10-24 at 2.43.14 PM.png]]
	3. Click on 'add files -> upload files'. Drag-n-drop the index.md note onto the upload pane. Once it's finished uploading, click the green 'commit' button at the bottom. Now go to step 5.
4. **Advanced** If you are familiar with using Git on the command line, you can **clone** the repository you generated **into your Obsidian folder/vault** ; it will turn up in Obsidian as a folder called `repo-name`. 
	1. **Move your notes** that you would like to make public to the `repo-name/docs` folder.
	    - Easiest way to do this would be using drag and drop within Obsidian
	1. Commit and **push** the changes. Github actions will take care of the rest, publishing your notes using [MkDocs](https://www.mkdocs.org/), with the [Material theme](https://squidfunk.github.io/mkdocs-material/). 
5. Go to `Settings > Pages` and select the select the **Source** as your `gh-pages` branch.

![](2021-11-22-22-52-49.png)

Give it a minute or two, and your website will be visible at `your-user-name.github.io/name-of-repo`.

## Updating the site

Move notes that you want to make visible to the world into your `website` folder (or the local repo folder, if you're using the advanced approach). Drop images into that folder, too, if you want the images to be visible on the web.  

Use github.com upload feature as described in step 3 to push your new materials online. 

If you want to change the look of your site, you'll need to consult the [mkdocs](https://www.mkdocs.org/) and modify the mkdocs.yml file as appropriate.

## Configuring your website

### How do I arrange notes as sections and pages?

By default, the sections and pages will follow the folder structure within `/docs`. The folders and sub-folders will show up as sections. Try not to have white spaces in your folder and file names, as these will be converted to HTML links. The webpage heading will be the same as the first-level heading in the markdown note.




