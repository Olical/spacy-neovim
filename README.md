# spacy-neovim

A base [Neovim][] configuration template inspired by [Spacemacs][].

Please fork and modify the repository to suit your needs, you can build your own Neovim on top of this (subjectively) cool starting point.

## Who's it for?

If you're currently using Spacemacs for [Clojure][] (or any other language, Clojure is just my favourite) and you feel like trying out Neovim, you may feel overwhelmed and alienated at first. You don't know where to start building your own Neovim configuration.

How do you structure it? What plugin manager do you use? What's airline? Who's tpope and why are they so great?

These are the questions the intended audience will probably be asking themselves.

## How do I get it?

 1. Clone your fork of this repository into `~/.config/nvim/`
 2. Execute `~/.config/nvim/sync.sh`
 3. ???
 4. Execute `nvim`
 5. Profit!

You'll want to run `sync.sh` whenever you change your `plugins.vim` list or if you just want to update all of your current plugins.

## Plugins?

Plugin management is provided by the wonderful [vim-plug][]. I've set things up so all you need to do is regularly run `sync.sh` to keep things up to date and alter `plugins.vim` to add or remove plugins.

To learn about the current plugins you can use the `:help` command in Neovim or just put the `username/repo` combination from `plugins.vim` into GitHub.

Configuration for your plugins should go under `modules/plugins/NAME.vim` where `NAME` is the exact repo name of the plugin. If you remove a plugin from `plugins.vim` but forget to remove the appropriate config file my script will warn you.

## Bindings?

Here's a selection of bindings that you may find useful coming from Spacemacs:

 * `<space>fs` - write the current buffer to disk
 * `<space>gs` - open [fugitive][], the awesome git interface (a bit like magit)
 * `<space>gl` - perform a git pull
 * `<space>gp` - perform a git push
 * `<space>pf` - search your files with [CtrlP][] and [Ag][] (a bit like projectile)
 * `<space>pb` - browse your current buffers in the same way
 * `<space><space>` - followed by any motion will fling you around the screen with [EasyMotion][]

There's way more to discover in the source of the [vim-better-default][] plugin, which is included already.

I highly encourage you to explore the plugins and source code to discover more, this list is far from exhaustive.

## Who's this from?

I'm a long time Vim user, JavaScript escapee, Clojure admirer and keyboard builder. I've been using Spacemacs for quite a while now but fancied playing with Vim again, so I thought I'd put what I feel is a good starting point up here for others to build upon.

Here's a little more of me around the internet for further context:

 * https://oli.me.uk/
 * https://twitter.com/OliverCaldwell
 * https://github.com/Olical

Feel free to throw opinions about languages and text editors at me or help refine this little project into something small yet powerful.

## Unlicenced

Find the full [unlicense][] in the `UNLICENSE` file, but here's a snippet.

>This is free and unencumbered software released into the public domain.
>
>Anyone is free to copy, modify, publish, use, compile, sell, or distribute this software, either in source code form or as a compiled binary, for any purpose, commercial or non-commercial, and by any means.

Do what you want. Learn as much as you can. Unlicense more software.

[unlicense]: http://unlicense.org/
[neovim]: https://neovim.io/
[spacemacs]: http://spacemacs.org/
[clojure]: https://clojure.org/
[vim-plug]: https://github.com/junegunn/vim-plug
[vim-better-default]: https://github.com/liuchengxu/vim-better-default
[fugitive]: https://github.com/tpope/vim-fugitive
[ctrlp]: https://github.com/ctrlpvim/ctrlp.vim
[ag]: https://github.com/ggreer/the_silver_searcher
[easymotion]: https://github.com/easymotion/vim-easymotion
