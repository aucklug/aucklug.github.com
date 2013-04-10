---
title: Editing, and creating, content for this website
layout: post
author: aki
authoruri: http://aki--aki.github.io
---

If you've got write access to the [aucklug/aucklug.github.com repository on GitHub][1], you can edit this website. It is built upon [Jekyll][2], a 
static site generator written in Ruby which powers thousands of websites, including many of [pages.github.com][3]. There's three ways to contribute content:

 - If you have Ruby installed, and are familiar with using git and the command-line, you can clone this website. If you want to preview your changes 
locally, you'll have to install Jekyll and run the local development server. The `_config.yml` file is set up properly enough that you'll be able to 
just invoke `jekyll` in the root of the repo and get started.
 
 - If you are comfortable with git, but not with Ruby, or if you just want to edit and create posts, you can do the same as above, clone the repo, but 
touch only the contents of `_posts/`.
 
 - Otherwise, you can use GitHub's web interface to make your changes. (( insert description here ))


There are a few rules to respect to be able to effectively edit posts.

 - The **filenames** are of the format `YYYY-MM-DD-simple-title-alphanumerics-and-hyphens-only.<markup>`. You can use [Markdown][4] or [Textile][5], 
so `<format>` can either be `.textile` for Textile or `.md` (most common), `.mkd` (rare), `.markdown` (verbose) for Markdown.
 
 - The posts contain **[YAML front-matter][6]**. This is a block delimited by `---` at the top of the file.
   
   The two most important values are `title: Something or other` which sets the post's title, and `layout: post` which sets what kind of post this is. 
The possible types are: `post` for a post/news, `event` for an event/announcement, `page` for a static page, and `default` to avoid all specific 
formatting (although I strongly discourage that!).

   Because the title is set in front-matter, you don't need to have a level 1 (`# Text` or `=====` underline in Markdown) at the start of a post. Just 
dive straight in.

 - Posts and events are shown in their respective sections in the sidebar of the site, and on their own archive pages accessible from the top 
navigation.


With that, you should be able to contribute content quite easily :)

(thanks to [passcod][7] for writing the majority of this for the UALUG site!)

[1]: https://github.com/aucklug/aucklug.github.com
[2]: http://jekyllrb.com
[3]: https://pages.github.com
[4]: http://daringfireball.net/projects/markdown
[5]: http://textile.thresholdstate.com/
[6]: https://github.com/mojombo/jekyll/wiki/YAML-Front-Matter
[7]: https://github.com/passcod
