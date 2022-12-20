This information is also in the [[1.A Demo Obsidian Vault|the obsidian vault I provided to you]] but I thought I should include it here as well.



<div style="position: relative; padding-bottom: 62.5%; height: 0;"><iframe src="https://www.loom.com/embed/f98e1bc894ae4b83b216b9d2e2195b2e" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>

We are going to configure Obsidian so that it can reach out onto the web and grab any of your [hypothes.is](https://hypothes.is) annotations from a website or a pdf you found online. It can:

-   Retrieve your annotations for a web article/web PDF'
-   Retrieve your annotations from a date
-   Open a URL in hypothes.is for annotation
-   Retrieve ALL user annotations for a web article/web PDF

Then,

-   If invoked in an empty document, descriptive front matter is output to beginning of the document, followed by annotations
-   If document already contains text, the annotations are inserted at the current cursor location

It's quite cool. So! Let's begin.

1.  I'm assuming you have a hypothesis account already. Make sure you're logged into your hypothesis account, and then click on this link: [https://hypothes.is/account/developer](https://hypothes.is/account/developer). This will take you to a page that looks like this: ![hypothesis developer key](https://github.com/shawngraham/obsidian-hist1900c-student-vault/blob/main/_media/hypothesis-developer-key.png?raw=true)
2.  Select and copy that entire key.
3.  Back  in obsidian, hit cmd+n or ctrl+n to make a new note.
4.  Don't worry about naming it. Now hit cmd + shift + H (on a mac) or ctrl + shift + H (on windows) to run the Hypothesis command.
5.  Paste your key into the pop up box. This will make a new file in your vault called `hypothesis config`. You can leave that where it is; don't mess with its insides. But that's the last time the Hypothesis code will ask you for it (unless you delete it, right? It's the key that unlocks the door to your online annotations, so you'd have to provide the key again if you deleted it here.)

Now you'll be presented with another pop-up box, asking you: ![hypothesis-modal.png](https://github.com/shawngraham/obsidian-hist1900c-student-vault/blob/main/_media/hypothesis-modal.png?raw=true) Select whichever one you want! You're now able to annotate websites and online pdfs with Hypothes.is, and import those results back here to Obsidian. ^c6c91a

[[Zotero|Let's get Zotero set up now]].