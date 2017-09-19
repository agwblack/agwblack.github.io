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
[Pages](https://jekyllrb.com/docs/pages/) (static pages such as your home page,
about page, that sort of thing) and [Posts](https://jekyllrb.com/docs/posts/)
(blog posts and the like, that get added over time).

To create this post I created a `_posts` directory and added the following file:

*TODO: get a post up and running*

*TODO: get a page up and running*

*TODO: Link to the posts from the home page*

*TODO: whats all this YAML front matter all about*
