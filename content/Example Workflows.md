---
publish: true
---
To conclude the tutorial we would like to offer some example walkthroughs for how to complete common tasks including adding, removing, hiding, revealing and linking to content. These sections are meant to function as a quick reference, for users who have already completed the above setup and understand the system well. 

>[!note]
> We've created this section as a separate page so that it can be easily bookmarked and used by instructors. If you're reading this from the main tutorial, then this is a lovely example of a transclusion!
### Adding and Removing Content

1. To add completely new pages to your site, open your content vault with Obsidian and in the file explorer on the left, right click and select “New Note”. Fill in the page with any content you wish to include referencing the Obsidian [basic formatting documentation](https://help.obsidian.md/syntax) as necessary. 
2. Making edits or adding to existing pages can simply be done by editing the markdown file in Obsidian. Deleting content can be done by deleting the entire file, or removing the content from the file just as you would in any text editor.
3. Once complete, you can view your site locally to check everything looks right before a deployment (see Building and Viewing Previews). 
4. To publish press Ctrl/Cmd+P and select the “Git: Commit-and-sync” command. Within a few minutes you should see the changes on your public site. Optionally you can login to Cloudflare to view the build process, monitor for errors and troubleshoot if problems occur.

### Hiding and Revealing Content

1. To hide content first ensure you have followed the instructions from the Adding Hidden Folders section. Then add a folder simply called “hidden”. Place the content you would not like published inside of this folder. 
2. Revealing content is as simple as removing it from the hidden folder.
3. View the site locally (see Building and Viewing Previews) and ensure that your hidden content cannot be reached by directly typing in the URL. Also confirm that unhidden content is accessible as desired. 
4. To publish press Ctrl/Cmd+P and select the “Git: Commit-and-sync” command. Within a few minutes you should see the changes on your public site. Optionally you can login to Cloudflare to view the build process, monitor for errors and troubleshoot if problems occur.

### Linking and Embedding Content

1. Linking to content can be done by using the wikilinks or markdown format although Quartz only supports embedding content in wikilinks format, and external links must be written in markdown format. Below is a quick reference for using wikilinks and markdown links formats.
  
##### Wikilinks Syntax

- `[[Path to file]]`: produces a link to Path to file.md (or Path-to-file.md) with the text Path to file
- `[[Path to file | Here’s the title override]]`: produces a link to Path to file.md with the text Here’s the title override
- `[[Path to file#anchor|Anchor]]`: produces a link to the anchor Anchor in the file Path to file.md
- `[[Path to file#^block-ref|^block-ref]]`: produces a link to the specific block-ref in the file Path to file.md

##### Embeds

- `![[Path to image]]`: embeds an image into the page
- `![[Path to image|100x145]]`: embeds an image into the page with dimensions 100px by 145px
- `![[Path to file]]`: transclude an entire page
- `![[Path to file#anchor|Anchor]]`: transclude everything under the header Anchor
- `![[Path to file#^b15695|^b15695]]`: transclude block with ID `^b15695`

Sourced from [https://quartz.jzhao.xyz/features/wikilinks#syntax](https://quartz.jzhao.xyz/features/wikilinks#syntax)  
##### Markdown Syntax
- `[Here’s the title override](Path to file)`: produces a link to Path to file.md with the text Here's the title override
- `[Here’s the title override](www.example.com)`: produces a link to [www.example.com](http://www.example.com) with the text Here's the title override
2. View the site locally (see Building and Viewing Previews) and ensure that your or embeds are working correctly.
3. To publish press Ctrl/Cmd+P and select the “Git: Commit-and-sync” command. Within a few minutes you should see the changes on your public site. Optionally you can login to Cloudflare to view the build process, monitor for errors and troubleshoot if problems occur.
