+++
showonlyimage = false
image = ""
date = "2018-01-16T19:56:17+05:30"
title = "Tutorial: Manually create a Markdown table of contents for your GitHub README"
weight = 55
+++

When I was learning Markdown, I practiced by reproducing a work sample that I originally created in Microsoft Word.

<!--more-->

It went perfectly in [StackEdit](https://stackedit.io)---even generated a linked table of contents with the handy little [TOC] marker. When I published my StackEdit file to a GitHub README, the beautiful table of contents was replaced with a disappointing "[TOC]" in plain text. No good!

The lack of a GitHub-Flavored Markdown table of contents marker seems to be a common complaint. It looks like there's at least one automated option ([DocToc](https://github.com/thlorenz/doctoc)), but I figured that I could learn something by working up a manual table of contents in Markdown.

I didn't find a step-by-step guide, so I patched together one way to do it from various Markdown cheatsheets and StackOverflow posts. Here's what I did.

Let's get this out of the way...yes, manually creating a table of contents in Markdown is a pain. If you regularly add and delete sections in your README file, it's even worse because you have to remember to update the table of contents too. The more headings your document has, the worse it gets. It's not realistic to manually create tables of contents for every GitHub README file.

**It does work, though**. We will focus on that part for right now!

Here's the original work sample created in Microsoft Word:

* [Sample Work Practice for Job Briefings](/samples/JobBriefingsWorkPracticeExample.pdf) (.pdf)

The table of contents on page 1 is what I wanted to recreate in Markdown for my GitHub README. My requirements were simple:

* Looks neat and organized.
* Clicking on the name of a section in the table of contents sends you directly to that section in the content itself.
* The idea was to use Markdown bulleted lists and inline links to create a table of contents that meets these requirements. The link text would be the title of the section, and the link would be to the corresponding section heading in the README file.

**Reminders**

Here's one way to make a bulleted (unordered) list in Markdown:

`* List item`

Here's how to make an inline link in Markdown:

`[Text to display](the URL)`

First, I wrote the file in Markdown. I followed the same organization as the original file, using # for the document title, ## for first-level headings, ### for second-level headings, and so on. My document had three levels of headings, so I went up to ####. Here's what that looked like in StackEdit:

![Screenshot of heading levels in a StackEdit Markdown file][1]

When I published the StackEdit file to a GitHub README, the same content looked like this:

![Screenshot of a StackEdit Markdown file when published to GitHub README][2]

After I published my Markdown file to GitHub, I was ready to manually add a table of contents. I went back to StackEdit to do the typing.

I made a bunch of inline link placeholders at the top of my document, after the title and document number. It looked like this:

```
[Text](link)

[Text](link)

[Text](link)

[Text](link)
```

...and so on.

I knew what to put in the [Text] part: the section titles! So I filled those in with all the ##, ###, and #### text in my document:

```
[Purpose](link)

[Scope](link)

[Work Practice](link)

[Daily Briefing](link)
```

...and so on.

What should go in the (link) placeholder? I had to go back to my GitHub file to find that information. In a GitHub Markdown file, if you hover the mouse over a heading, a little link icon appears:

![Link icon next to heading in GitHub Markdown file][3]

While you are hovering the mouse over that little link icon, look at the bottom of the browser window (the status bar). You will see the target URL for the header item's link:

![Target URL for link to heading in browser's status bar][4]

If you click the little link icon, the browser will reload. The target URL will be in the address bar, and the document will "snap" so that the selected heading is at the top of the screen. This heading-specific URL is what goes in the (link) placeholder:

```
[Purpose](https://github.com/hillaryfraley/jobbriefings#purpose)

[Scope](https://github.com/hillaryfraley/jobbriefings#scope)

[Work Practice](https://github.com/hillaryfraley/jobbriefings#work-practice)

[Daily Briefing](https://github.com/hillaryfraley/jobbriefings#daily-briefing)
```

...and so on.

These links followed a predictable pattern (the heading name, lower case, with hyphens in place of spaces), so I only copied and pasted the link for the Purpose. For Scope and everything after, it was easier for me to re-paste the "Purpose" link and just replace "#purpose" with "#scope" and so on for the rest of the headings.

Here's what it looked like in StackEdit after I had all the inline links set up:

![List of inline links in Markdown][5]

Not bad! I still wanted to show the headings in hierarchy instead of a flat list, though. This is where the bulleted (unordered) list marks came in. I had to fiddle with them, just adding and removing blank lines and using the different bullet symbols until I found something I liked.

Here's the finished Markdown in StackEdit:

![Finished manual table of contents in Markdown on StackEdit][6]

The last task was publishing the final to a [GitHub README](https://github.com/hillaryfraley/jobbriefings).

It's not quick or automated, but it IS a neat, organized, clickable table of contents in a GitHub README file!

#### Tools

* GitHub
* Markdown
* StackEdit
* Sublime Text

[1]: /img/portfolio/MarkdownTOC1.jpg
[2]: /img/portfolio/MarkdownTOC2.jpg
[3]: /img/portfolio/MarkdownTOC3.jpg
[4]: /img/portfolio/MarkdownTOC4.jpg
[5]: /img/portfolio/MarkdownTOC5.jpg
[6]: /img/portfolio/MarkdownTOC6.jpg

