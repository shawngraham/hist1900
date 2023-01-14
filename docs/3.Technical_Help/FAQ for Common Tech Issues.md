
## I hit ctrl + shift + h and nothing happens

This seems to affect PC users. The issue here seems to be that sometimes, for PC users, the configuration of the command for hypothes.is note extraction has been rest.

Open the Obsidian vault settings by clicking on the cogwheel icon at bottom left. Then, click on the 'Templater' settings at the bottom left (as in the screenshot below). You'll need to adjust the `template folder location` setting: it should be `_ancillary_code_do_not_touch`. 

Then, under `template hotkeys`, hit the + button to tie a hotkey to `_ancillary_code_do_not_touch/hypothes.is.md`. 

![[Screen Shot 2023-01-10 at 1.26.06 PM.png]]

 Then, on the next page it'll say `Templater: Insert _ancillary_code_do_not_touch/hypothesis.md blank` Click on where it says `blank` and type: ctrl+shift+h . Then you can hit the x to close the dialogue.
 
 ![[Screen Shot 2023-01-10 at 1.26.16 PM.png]]

Now you're configured, and when you type ctrl+shift+h you'll get the hypothesis extraction dialogues.

There is a video on the [[Import Your Hypothesis Annotations]] page showing the whole process in action for how this tool is supposed to work.


## I get the error `couldn't retrieve template files from templates folder _complex templates_`

This seems to be happening to folks on PCs. Two places to check. 

+ check that the 'templater' configuration is set up as in the screenshots above for the previous question - it should be looking for the hypothesis.md code file in the folder `_ancillary_code_do_not_touch`
+ check that the **templates** configuration is set up as in the screenshot below where the `template folder location` is set to `_note_templates`:

![[Screen Shot 2023-01-12 at 4.46.51 PM.png]]

## When I try the Zotero annotation extraction, I get an empty bibliography error

There's a couple of different things that might've gone wrong here. First thing, go to the community plugins general page (hit the cogwheel icon to bring up preferences, then click on 'community plugins' under options at the top left of the dialogue box). 

Click on the button that says 'check for updates'. 

If it finds updates, click on 'update all'.

**NB!!!** When you search for the zotero - extract annotations command and run it, **check the `1-inbox` folder when it seems to finish**. If it has been successful, you'll find a note there with all your annotations extracted. *You might still get an error message* but this is one you can ignore.

The other zotero commands require you to have a note open and the cursor blinking where you want to insert a bibliographic reference, etc. So if you run one of those commands *without* an open note, you'll get an error.

There are two videos on the [[Zotero]] page showing two different ways to get your annotations using the Zotero extractor commands.

## When I try to use the Zotero - Full Reference command, I get an empty bibliography error

This one's my fault. My code for zotero extraction is set up to format things in the format preferred by the Journal of Computer Applications in Archaeology. There are two ways to solve this.

With Zotero turned on and running on your machine, click on this link: [https://www.zotero.org/styles/journal-of-computer-applications-in-archaeology](https://www.zotero.org/styles/journal-of-computer-applications-in-archaeology) A dialogue box will open asking if you want to add this to your citations styles in Zotero. Say yes.

*If that link doesn't prompt a dialogue box* you'll find instead a file in your download files called `journal-of-computer-applications-in-archaeology.csl`. With zotero open in the background, double-click on that file; your computer will know to use Zotero to open it and will ask you if you want to add that style to Zotero. Say yes.

This should solve the problem.

Your alternative is to open the zotero integration plugin configuration in Obsidian. Hit the cogwheel, bottom left, the scroll down until you see zotero integration. The, under 'Citation Formats' there are two boxes where you can set the style for making a citation, and for making a full reference. Start typing where it says 'Journal of Computer Applications in Archaeology' to change it to eg. Chicago, APA, Turabian, whatever. Then hit the 'x' when you're done. Note - you gotta make sure in Zotero that whatever you change it to is already there. But Chicago, APA, Turabian should probably be there by default. If they're not, you'll get the same error message again.  You can search for citation styles [here](https://www.zotero.org/styles/).


## The browser won't let me download the Better BibTex plugin for Zotero 

Different browsers have different default security settings. Try a different browser, or right-click and save as this link: [https://github.com/retorquere/zotero-better-bibtex/releases/download/v6.7.46/zotero-better-bibtex-6.7.46.xpi](https://github.com/retorquere/zotero-better-bibtex/releases/download/v6.7.46/zotero-better-bibtex-6.7.46.xpi).

## My Mac won't let me install Obsidian or Zotero

Sometimes Mac security settings try to stop you from opening software downloaded from places other than the Mac store. Download the file, and then find it on your machine using Finder. Hold down the ctrl button while clicking on the file. A contextual menu will appear; one of the options will be 'open'. A security warning will appear, but it will have a button on it saying something like 'open anyway'. Click and you're good.