# Men's Rights 101 Website
This repository reflects the live version of [MensRights101.com](http://mensrights101.com). By using GitHub for the website, anyone is free to contribute. Using GitHub also helps to prevent vandalism, as any changes are made in the form of pull requests, and they would need to be approved.

## How to contribute
The website is in need of writers. At the moment, those are the only pull requests I'll accept. Do not make design changes.
* Before creating a new page in the `_pages/issues/` folder, first decide if it would be better to just edit or add a new section to an existing page.
* Refer to the sample page code below to ensure it's structured correctly.
* Follow the content guidelines also listed below.
* GitHub allows you to edit Markdown (.md) files right here on the website. But you can't edit the ones in this exact repository. Instead, you must fork the project, edit/add the .md files there, then submit a pull request. I will receive the pull request, review what changes you've made, then decide whether to merge them into the live site or not.
* Before making any changes, ensure you've fetched the most recent version of this repository. If you make changes on an older version, it will be difficult to merge even if the edits you made are awesome.
* You may also submit changes to the content of `index.html`, and the markdown files inside `_pages/faq` and '_pages/about'.
* For Markdown basics, refer to [this website](http://daringfireball.net/projects/markdown/basics).
* If all of the GitHub stuff is too complicated, feel free email your writings via email: mensrights101@gmail.com

## Content Guidelines
* The goal of the Men's Rights 101 website is to be strictly informational. The "101" suggests that the information should be written in a simple and neutral language. Assume the reader does not know advanced gender studies terminology. The website should be accessible to middle school and grad school students alike.
* It is not a place for ranting or complaining, even if such things are justified. This is common in the MRM forums, but it should be avoided here. This site aims to be professional and tactful; not an echo chamber.
* The website is about the Men's Rights Movement (MRM). Nothing else. Do not compare the MRM to other movements or ideologies. Do not cover the history, positives, or negatives of other groups either. This will help you avoid the no ranting rule.
* Avoid being preemptively defensive. It's common knowledge that the MRM is not very popular, despite its overwhelmingly egalitarian members. This may cause urges to phrase things in the defensive, but don't. Just state information.

## Sample Issues Page Notes
* The filename must include a date. The site might not actually use it, but the software requires it. So filenames are in the format of `YYYY-MM-DD-title.md`. The `title` is what will be used for the URL. Just use whatever date is already in the filename, don't update the date. If creating a new file, use the date that you submit the pull request. In the future, once there's a fair number of articles, the dates will be used to sort the order that articles appear on the page.
* Note at the top of each .md file, there's a section surrounded by 3 dashes above and below. This is called "Front Matter". This is where you edit the page title and the excerpt. The excerpt will be a short summary no longer than a small paragraph. For pages in the Issues part of the website, also ensure that `category: issues` is present.
* Next is the page title with one hash (`#`). Right after the # is `{{ page.title }}`. Leave that there. It repeats the same title you typed
* After the title is a short summary of the whole page, which should be very similar to the excerpt, but may be longer. You can repeat the same paragraph as the excerpt with `{{ page.excerpt }}`.
* After the summary is a menu of links to the sections within the page. Each menu item begins with an asterisk (`*`). Then a link to the section, in the format of `[Section Title](#section-title)`. The part inside the parenthesis will match the part inside the brackets, except in lowercase and with a hyphen in place of spaces. Don't forget the hash.
* After the menu are the sections. Each section includes a title prepended with two hashes, in the form of `## Section Title`. Be sure to use the same name here as you did for the links in the menu. Following the title is one or more paragraphs, separated by spaces.
* Any images that accompany an article should be placed in the existing `img` folder, and titled based on the page it's being used in, such as on page `_posts/issues/themedia`, the very first image should be named like `img/issues-themedia-1.jpg`. Do not link to external images. Uploading an image is a bit more involved than editing the .md files directly on GitHub. You'll have to actually clone a local repo with Git and do your changes there. If that is beyond you, explain and link to what image you'd like inserted when creating the pull request. Images must not be copyrighted.
* The final section of any Issues page will be the Sources. This is the only section where you may have external links. And that's all that should be here, links. The links will be with HTML `<a></a>` tags, and have an id that's a number. Use the exact title of the article you're referencing. To cite one of these sources within the content, create a superscript markdown link with the right number, such as `<sup>[2](#2)</sup>`

## Sample Issues Page Code
Here is what the Markdown Code of an issues page should actually look like.
```
---
title: This is the Article Title
excerpt: A brief summary of this page. No more than a few sentences.
category: issues
---
# {{ page.title }}

This intro paragraph should be the same as the excerpt, maybe a little longer, but still just a brief summary. Alternatively, repeat the excerpt exactly with `{{ page.excerpt }}`.

* [First Section](#first-section)
* [Another Section](#another-section)
* [Sources](#sources)

## First Section
A paragraph. Lorem<sup>[1](#1)</sup> ipsum...

Another paragraph. Lorem ipsum...

## Another Section
A paragraph. Lorem ipsum...

Another<sup>[2](#2)</sup> paragraph. Lorem ipsum...

And another paragraph. Lorem ipsum...

## Sources
1. <a id="1" href="http://example.com">An External Article</a>
2. <a id="2" href="http://github.com">Another External Article</a>

```

## Open Source
This site and any content you submit to it will be considered public domain. It's likely that people will link to and cite the content on the site with the site itself as the source. If you submit excerpts or cites from other sources, be sure to cite the source as described previously in this README.
