# Setting Up Jekyll and GitHub Pages

I was recently inspired to make another attempt at blogging again, inspired by
my friend [Dan Blank](http://danblank.co.uk). I looked at using WordPress as he
does but WYSIWYG is not really my bag. Dan sent me [this
link](http://www.firozansari.info/no-wordpress-for-my-blogs-again/) about the
benefits of static website generators, and I started looking into how to setup
Jekyll and GitHub pages. This post serves two purposes: it is an accounting of
what I had to do to get it set up correctly, and a practice first post on which
to test.

## Setting up Pages

GitHub has good introductory documentation on setting up pages. I was quickly
able to get a basic "Hello World" page up, with only this file in my
repository:

    $ ls
    index.html

    $ cat index.html
    Hello, world

Basic, committing and pushing but it works:

*TODO: insert picture*

## Selecting a theme

GitHub It also has some basic stuff on setting up a theme (I went with *Tactile*).  
I got rid of index.html and created index.md:

    $ ls
    index.md

    $ cat index.md
    # Hello, world

    Is anyone there?

Things are starting to look prettier at this point:

*TODO: insert picture*

## Creating a post

At this point I started looking at the [Jekyll
documentation](https://jekyllrb.com/docs/home/). Jekyll distinguishes between
[pages](https://jekyllrb.com/docs/pages/) (static pages such as your home page,
about page, that sort of thing) and [posts](https://jekyllrb.com/docs/posts/)
(blog posts and the like, that get added over time).

To create this post I created a `_posts` directory and added the following file
in it:

    $ ls _posts
    2017-09-19-setting-up-jekyll-and-github-pages.md

Note that the format of this file name is important. It needs to have the date
first, in the format shown, followed by the title.

Adding this file into our repo and pushing it to GitHub, we can now go and
visit this page. As described [here]() Jekyll will create a path based on the
filename. In this case, it is
https://agwblack.github.io/2017/09/19/Setting-Up-Jekyll-And-GitHub-Pages.html.
You can see how this directly derives from the from the name of the file.

*TODO: insert picture*

Starting to look like an actual website now!

## Customising the Theme

*TODO: fix font in code snippets*

## Linking to our posts

*TODO: Link to the posts from the home page*

## Drafts

Throughout this process we've been updating our post as we go. But that means
that it has been live the whole time, changing with every commit. Most of the
time it is undesirable to be leaving an unfinished post live on the internet.
But we still want all the version control benefits that git provides when we're
working on a post. Jekyll accounts for this. Keep unfinished posts in the
`_drafts` folder. These files do not need the date in their title, since the
date they are posted hasn't been determined yet.

*TODO: how to test these files before pushing them*
