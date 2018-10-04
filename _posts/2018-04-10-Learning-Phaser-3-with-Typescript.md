# Learning Phaser 3 with Typescript

This post sets out my motivation for learning Phaser 3 using Typescript, in preparation for my next game jam (hopefully Ludum Dare 43, in December 2018).

[Phaser](https://phaser.io/) is an open source framework for making games, with
a focus on deploying to the browser.

[Typescript](http://www.typescriptlang.org/) is a typed superset of Javascript that compiles to regular Javascript.

Both technologies are open source, which is a key consideration in my using them. I'll perhaps discuss why I consider this important in a future post.

## Why Phaser?

I became aware of phaser a few years ago when I briefly got excited about Javascript. Since then that excitement has faded, but I'm still interested in Phaser. This is because I recently took part in my first game jam, Ludum Dare 42 (you can see our entry [here](https://ldjam.com/events/ludum-dare/42/bunnies-out-of-space). I was pleased with what we managed to achieve although I don't think the final game was that much fun. I'll save a proper post-mortem discussion of that whole experience for another post.)

One thing really stood out to me when playing other people's games as part of the review phase of LD42: it was a lot easier to play people's games if they had a web version. No downloading, no cryptic segfaults, and so on. This is doubly true for a Linux user such as myself, since many games did not publish a Linux version. 

But the framework we used to produce our game ([Love2D](https://love2d.org/)) does not properly support [web deployments](https://love2d.org/wiki/Game_Distribution#Distribution_on_the_web). So I was keeping my eyes peeled for something with first class web support.

Then a couple of days ago, Mike at [GameFromScratch](https://www.youtube.com/user/gamefromscratch) (one of my favourite YouTube channels) published a [this video](https://www.youtube.com/watch?v=fu89TGKNFb0) on the new release of phaser, version 3.14. This recalled my earlier interest in Phaser, and I started looking into it.

## Why Typescript?

Over the years, I've explored many different programming languages. One of the things I've come to realise is that I simply just prefer statically typed languages, at least for non-trivial projects. This is especially apparent to me with my day job where I use both C++ and Python on a daily basis. I love how quickly you can throw something together in Python, but maintaining a complex piece of software written in it gets tricky.

Javascript suffers from the same problem. As I found it in LD42, where I was using Lua, there are certain classes of bugs that you can miss with dynamically typed languages, especially in the pressure-cooker of a 48 hour game jam environment. I had already been considering moving to [Rust](https://www.rust-lang.org/) for my next game jam (probably using the [ggez](http://ggez.rs/) framework, which is inspired by Love2D), because I was so fed up with the pitfalls of dynamically typed languages.

But ggez does not yet have web support (although [it's coming](https://github.com/ggez/ggez/issues/71)). So we're back to Phaser, but this means Javascript (which is really quite similar to Lua in many ways). I guess I'm stuck.

Except it turns out that Typescript is a thing. This an open source Microsoft project that let's you write typed javascript, then run it through a compiler that outputs pretty readable javascript. You can learn the basics of it [here](https://learnxinyminutes.com/docs/typescript/). This is a step beyond the likes of [mypy](http://mypy-lang.org/) and [type annotations](https://docs.python.org/3/library/typing.html) for Python. What's more, Phaser provides Typescript declarations for use in your Typescript programs.

Problem solved?

## The Missing Resources

Unfortunately, there are not many tutorials for Phaser 3 (although here are [some](https://phaser.io/learn/community-tutorials])), or for Phaser with Typescript (although here is [one](https://phaser.io/tutorials/how-to-use-phaser-with-typescript)). And there are even fewer for Phaser 3 with Typescript, although I just stumbled across [this](https://github.com/digitsensitive/phaser3-typescript) which looks to be a very useful resource.

Anyway, I have a basic game design I want to implement, and I will probably follow up with my progress in a little while.
