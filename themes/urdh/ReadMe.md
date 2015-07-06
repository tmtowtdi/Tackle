# urdh

urdh provides a pretty simple prompt, with support [Git][] and [Mercurial][].

![urdh prompt screenshot][screenshot]

## Requirements

### vcprompt

You **must** have [vcprompt][] installed to use this theme, which on Mac OS X can be done via:

    brew install vcprompt

Why the hard requirement? Determining whether the current working directory is under version control is cumbersome and adds latency to the prompt. It doesn't make sense to have a slow terminal prompt on a 3+ GHz machine, right? [vcprompt][] is a tiny C program that is also extremely fast, which makes it perfectly suited to making this determination.

If you only use Git, then you're all ready to go.

### hg-prompt

If you use Mercurial, you'll also need to install [hg-prompt][], which populates the prompt with relevant information when the current working directory is inside a Mercurial repository.

[hg-prompt]: http://sjl.bitbucket.org/hg-prompt/
[Git]: http://git-scm.com/
[Mercurial]: http://mercurial.selenic.com/
[screenshot]: http://i.imgur.com/zoa85vj.png
[vcprompt]: https://bitbucket.org/gward/vcprompt
