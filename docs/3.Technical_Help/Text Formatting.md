# Text Formatting 

You can have lists like this

```
- first
- second
- third
```

Or checklist lists to

```
- [ ] ==Get==
- [ ] things
- [ ] ~~done~~
```

You can make headers using the `#` like this:

```
# Really Big Header
## Level Two Sub Header
### Level Three Sub Header
```

If you forget the space between the `#` and the text, congratulations, you've made a 

```
#tag
#tag/subtag
```

In the right-hand sidepane in Obsidian, you can also view a tag explorer to help you navigate your materials.

Within obsidian, you can drag and drop images right in. This will create a copy of the image inside your vault. Then, start typing:

```
![[ 
```

and the file selector will open. Select the filename for the image you want, hit enter, and ta da!

For notes and images that you want to push online, just make sure that the images are in the main `website` folder (if you're a github newcomer) (or the `\docs\` folder if you're using git at the command line and have cloned the repository into your vault, in which case you can git commit and git push everything). 

THEN, just drag and drop the images and notes via the 'upload files' button on Github, when you are on the `\docs\` subfolder in your repository.

For folks comfortable with tweaking things, there is more formatting options for your eventual webpage [here](https://squidfunk.github.io/mkdocs-material/reference/formatting/#highlighting-changes) (but note that these will not render within Obsidian on your machine).