+++
author = "Douglas Cueva Jr"
title = "Starting out with Vim"
date = "2021-05-28"
description = "Beginning Vim without fear."
tags = ["Vim",
"beginner",
"code",
"command line",
"terminal",
"text editor"]
+++

# Vim

Probably one of the most notorious text editors is [Vim](https://www.vim.org). As someone that's used to text editors like VS Code, Vim presents the opportunity to feel like a ninja when editing code. 

If you're not familiar with Vim, the text editor, but have heard about it, then this is the post for you. 

Over the past week, I've taken a LinkedIn course about Vim and have begun using it in my projects and have found it to be enjoyable, so, I'd like to share what I've learned.

This tutorial will get you started slowly, so as not to scare you away from this text editor. 

There is a lot to learn, and a lot of Vim is memorizing commands so you can do what you want, but I believe that easing into things and finding a real-world use to apply what you've learned is most helpful.

So, by the end of this post you will have:

1. Edited and saved a text file using Vim.
2. Quit Vim

### Vim's Philosophy

I would sum up Vim's philosophy like this: the text editor at your fingertips.

### Assumptions

This tutorial assumes you have some proficiency with the command line, shell, or terminal.

I also assume you've downloaded and installed Vim. [Check out Vim's website for how to install it on your operating system.](https://www.vim.org/download.php)

For this tutorial, I'm using the [Fish shell command line](https://fishshell.com), but this should work with zsh, bash.

My computer is running macOS Big Sur 11.4

# Normal Mode and Insert Mode

Since Vim is an editor that opens up within your bash terminal, you might be wondering how viewing a file versus editing one work. Well, Vim has various modes that let you switch between viewing a file and editing one.

To demonstrate, create a file in an empty folder (that way it's easy to locate in your terminal), called *text.txt*.

You can create this file the old fashion way, if you'd like, by right-clicking and select "New File", or using the touch command on your terminal. There is a way to create any file and automatically open it with Vim from the command line, but I will go over that in another tutorial.

Now, you'll want to open up your command line, or terminal, and change into this folder you created. I've named mine Vim, and it's on my desktop. 

Within the Vim directory you'll see the newly created *text.txt* file, which is an empty text file.

Alright, we're going to open this text file using Vim. To do so, type the following command.

```bash

vim text.txt

```

You'll be dropped into the Vim text editor within seconds.

You've done it. You've begun using Vim! 

Since this file is empty, you won't see anything, but most of the time you'll be working with files that have content. We'll be adding our content here, but only do so much as to get you comfortable with using Vim.

Now, when Vim opens up a file, it opens it in View mode. In View mode, you can navigate a file, use regex to find certain words, and many other things.

Since we don't have much in this file, we're going to add content so we can learn some basic navigation skills with Vim.

Let's get out of view mode and go into *insert* mode. 

In insert mode you can delete words, add words, and more. 

We're going to add some words to this document. To do this, press the letter "i" on your keyboard.

If you notice on the bottom left, the word "insert" appears in all caps. This means you're in insert mode. 

Go ahead and type something. 

I wrote the following in my text file:

```
Hola, mi nombre es Douglas
y a mi me gustan las pupusas.

```

# Saving a file with :w

Now we want to save this file. Let's exit insert mode and go back into view mode where we can save the file. To do this press the **escape key** on the top left of your keyboard, or **ctrl + c** if you don't have an escape key. 

The bottom left of your screen shouldn't say insert anymore. It should be empty. This is how you know you're in View mode.

Now we can save the file. Type the following command and then press enter:

```bash

:w

```

This command saves the file (or 'writes' it). There are similar commands that will close out a file after you've saved it (:wq) but for our purposes this command is enough.

Now would be a good time to navigate your file. Since we're in View mode we can easily do this by pressing the h key, which moves you to your left. 

If you have two lines of text, as I do, you can move up with the j key. Move back down with the k key, and then move right with the l key. Try it out.

You can point and click to get to where you want, but the point of Vim is to avoid the mouse and use what's directly available at your fingertips. There's a great website that helps you get used to moving around with Vim called [Vim Adventure](https://vim-adventures.com).

# Quitting Vim with :q

We've done enough with this file and we want to exit the file and the Vim editor. 

To do so, we must remain in View mode and enter a command similar to saving this file. 

Go ahead and type the following command and press enter:

```bash

:q

```

Congratulations, you've exited Vim! 

If you haven't seen the funny memes about trying to exit Vim you can do so now with the assurance that you know how to exit Vim.

# Conclusion

Getting to know Vim and being comfortable with it takes time so, start small. 

I've used it while learning Hugo, the static website generator, editing the configuration files and markdown files. 

I haven't used it for large projects yet because I want the basics to feel natural, but my knowledge is compounding because I need more from it.

I hope this tutorial inspires you to check it out and know a little bit about it.

# Recommendations

If you want more, check out the book [Mastering Vim Quickly](https://www.amazon.com/Mastering-Vim-Quickly-WTF-time/dp/1983325740/ref=sr_1_4?dchild=1&keywords=mastering+vim&qid=1622393118&sr=8-4).

I also recommend the website [Vim Adventures](https://www.amazon.com/Mastering-Vim-Quickly-WTF-time/dp/1983325740/ref=sr_1_4?dchild=1&keywords=mastering+vim&qid=1622393118&sr=8-4).

I enjoy reading the wiki page of anything existence, and you can find [Vim's wiki page here](https://en.wikipedia.org/wiki/Vim_(text_editor)).

Lastly, check out their [website to see what they're all about and the cool charity work they do](https://www.vim.org).