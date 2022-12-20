[Zotero](https://zotero.org) is a very powerful reference manager and pdf reader/annotation environment. We are going to set up Zotero so that when you encounter material online, or in library catalogues, or in academic databases, it will ingest that material with the proper bibliographic information.

Once you have some articles in Zotero, you can also annotate them while reading them - highlight with different colours, and leave notes stuck all over them.

I have already configured Obsidian for you so that you can get it to call over to Zotero and extract the citation, the bibliographic reference, or the annotations for you. This was always the hardest part of reading online - liberating our annotations! So here's what you have to do.

## Getting Zotero Set Up

1.  Go to [Zotero](https://www.zotero.org/download/) and install BOTH the Zotero for your desktop AND the Zotero Connector for your browser. The first is the actual reference management platform, the second is the piece of code that lets your browser sense when there is bibliographic metadata & pdfs on a website (it adds a button to your browser - press it and boom, the material is downloaded into Zotero. Most of the time.)
2.  Now get the `Better BibTex` plugin for zotero. It is available [here](https://github.com/retorquere/zotero-better-bibtex/releases/latest) You want to click on the file ending with 'xpi' to download it. ![better bibtex link](https://github.com/shawngraham/obsidian-hist1900c-student-vault/blob/main/_media/better-bib-tex-link.png?raw=true)
3.  Then, in Zotero, you'll need to install that plugin: 
	1. In the main menu go to Tools > Add-ons 
	2. Select ‘Extensions’ 6. Click on the gear in the top-right corner and choose ‘Install Add-on From File…’
	3. Choose .xpi that you’ve just downloaded, click ‘Install’
	4. Restart Zotero

Phew! What this plugin does is it facilitates the creation of 'citation keys' for your references. You can think of these as unique knicknames that will instantly identify one reference, and one reference only. Imagine you had three articles by me, all published in 2022. Things could get confusing. But with BetterBibTex installed in zotero, when you drop my three pdfs into your zotero main panel, BetterBibTex will automatically rename them to `graham2022a, graham2022b, graham2022c`.

THEN, when we create notes here in Obsidian, your notes can be tied back directly to the source without confusion. That's actually a big deal; making notes and losing track of where they come from has driven many a grad student mad.

## Importing your notes from Zotero to Obsidian

As I said, I've already pre-configured this vault with everything you need to import new materials. Let's try something out. Make sure Zotero is open on your machine before we do this next bit, and make sure you've imported an article or two in there so we have something to work with. If you don't have anything yet, go to the Vannevar Bush article in your browser, hit your Zotero import button to ingest it: ![import-button.png](https://github.com/shawngraham/obsidian-hist1900c-student-vault/blob/main/_media/import-button.png?raw=true) but know that the icon _changes_ depending on the kind of resource. The article metadata will appear in your Zotero library. _Now_ we do the next bit.

In Obsidian, make a new note with cmd+n or ctrl+n.

Then, hit cmd+p or ctrl+p to open the 'command panel'. ![command-panel.png](https://github.com/shawngraham/obsidian-hist1900c-student-vault/blob/main/_media/command-panel.png?raw=true) 
Start typing 'zotero'. It will bring you up a series of commands;![zotero-commands.png](https://github.com/shawngraham/obsidian-hist1900c-student-vault/blob/main/_media/zotero-commands.png?raw=true) the two that are most useful for us (you can explore the others later) are 'Annotation Extraction' and 'Full Reference'. Select 'Full Reference'. The red zotero citation search bar will appear; start typing the name of a paper you might have in there - eg, B..U..S.. H and then select the reference. ^78e9e7

Boom! The full reference appears.

Now let's make some annotations on a pdf _in_ Zotero. A paper of mine that you can practice on is available through the Humanities Commons, called: [Fleshing Out the Bones](https://mla.hcommons.org/deposits/item/hc:19553/) . Go to that link in your browser. Hit the 'Save to Zotero' button (notice that the icon has changed slightly). Now, in Zotero, you will have the full bibliographic information _and_ the pdf of the paper: ![fleshing-in-zotero.png](https://github.com/shawngraham/obsidian-hist1900c-student-vault/blob/main/_media/fleshing-in-zotero.png?raw=true)

Double click on the pdf, and zotero's pdf reader will open the paper. Make some annotations. Highlight passages of text with different colours. I'd suggest using the following colours (it's what my code is set up for) to indicate _why_ you're making an annotation: ^1760dc

YELLOW: confusion/questions 

GREEN: agree 

RED: diasgree 

BLUE: definitions/concepts 

PURPLE: relevant/important

Explore the options for marking up that page. Everything saves automatically.

Just make a few. Then, back here in Obsidian, we're going to hit cmd/ctrl + p to bring up the command palette, then type Zotero to bring up the zotero commands, then select 'Annotation Extraction.' The familiar red zotero bar will come up for you to search for the article we want, so type in 'graham' or whatever. When you find it, hit enter. This will trigger the annotation extraction code; after a moment, the pop-ups will have disappeared. **Look in the `1-inbox` folder**:

![annotations-extracted.png](https://github.com/shawngraham/obsidian-hist1900c-student-vault/blob/main/_media/annotations-extracted.png?raw=true)

And if you click on that note, you'll find all of your annotations there, with headings according to the colour you used to annotate.

One last thing - there's a command called `zotero-integration: insert notes into current document`. This _doesn't_ insert your _annotations_. Rather, over in Zotero, if you click on an item, there's a tab called 'Notes'. Within Zotero, if you right-click on a pdf that you have annotated, and select 'add note from annotations', your annotations will be transfered to that 'Notes' tab. _Then_ over in Obsidian you use the `zotero-integration: insert notes into current document` command, _those_ notes are copied over.

## Two more videos of the vault in action

In the following video, I show how annotations made in the Zotero pdf reader can be imported directly into the vault.

<div style="position: relative; padding-bottom: 62.5%; height: 0;"><iframe src="https://www.loom.com/embed/01563c07b9bd4fa3aadff39ca018b399" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>

In this video, I show how annotations made in the Zotero pdf reader can be copied into the 'notes' pane *within* Zotero, and *then* copied into Obsidian. The difference in these two approaches comes down to which final output you prefer.

<div style="position: relative; padding-bottom: 62.5%; height: 0;"><iframe src="https://www.loom.com/embed/c0c612eab06c472abf7b557dfe435b77" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
