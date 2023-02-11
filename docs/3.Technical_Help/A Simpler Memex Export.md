
Folks, I have tried to make the process of putting stuff online as simple as possible for you. You might not agree that things have been very simple... but on the other hand, you **have** learned a lot about github!

A new plugin for Obsidian has just been released that can turn your individual notes or a whole folder or the entire vault into webpages (.html files). This simplifies **everything** considerably. You might want to try it out; you don't have to. If you've got our existing template working, just keeping dropping your notes into the /docs/ folder there. 

But if you'd like to try something else.... read on.

This is what you'll end up with: [https://shawngraham.github.io/simpler-memex/](https://shawngraham.github.io/simpler-memex/)

![[simpler-memex-screenshot.png]]

## Add 'webpage html export' plugin to your Obsidian Vault

- go to your 'community plugins' settings page
- hit 'browse' for community plugins
- search for 'webpage html export'
- hit install
- hit enable

## Configure its settings

- Make sure the settings look like this:

![[configure-webpage-export-settings.png]]

## Export your 'website' subfolder

- make a new, empty folder on your computer. Maybe on your desktop, and call it something like, 'memex-export'. You're going to get the plugin to put all of the html files in there.
- Right click on your 'website' subfolder in your obsidian vault. This subfolder, remember, is where you've put the notes that you want to move online (in the screenshot, I renamed my folder 'website' to 'move-online' by the way, just to make it clearer to Future Me).
![[right-click-export.png]]

In the pop-up, make sure you turn on these options:

![[export-to-html-last-settings.png]]

- Hit the 'export' button. It will ask you which folder to save everything to; select that new empty folder I suggested you put on your desktop.

A lot of stuff will seem to happen as the plugin pages through your notes, turning each one into nicely formed html. Congratulations!  You now have a folder filled with html. The last step is to put it online. And this is where things get comparatively super easy (compared to the template approach).

## Move your webpages online

- Create a new repository on github. Make it 'public'. Add a README file.

![[new-repo-to-make.png]]

- on the 'code' tab for your new repo, you'll see there's a button marked `main` with a dropdown button. Press that.
- type exactly `gh-pages` into the 'find or create' box that opens

![[make-gh-pages-branch.png]]

- Click on `Create branch: gh-pages from 'main'`.

Github will copy all of your html from the `main` branch - where you first uploaded everything, and will start to make all of your html files available online. Congratulations, you're done! 

You can click on the 'actions' button to see when it's finished, but your memex will now be online  at an address following this pattern: `your-username.github.io/name-of-your-repository`

Now that was easy!

## Updating your content

When you go to update your material, the easiest approach is to

1. make sure your note is in the subfolder in your Obsidian vault where you gather together the materials you want to make online (this is so the eventual interlinkages between notes work properly)
2. make sure your memex-export subfolder on your desktop is empty again
3. in obsidian re-export your subfolder as before (right-click, hit export as html)
4. on github **make sure you click on 'branches' and select 'gh-pages'** THEN you drag-and-drop your materials in.

![[make-sure-gh-pages-branch.png]]


(for those who are interested, you can set the default branch of your repository to `gh-pages` by following [these instructions](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/managing-branches-in-your-repository/changing-the-default-branch))