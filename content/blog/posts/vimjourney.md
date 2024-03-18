---
title: My (Neo)Vim Journey (so far)
type: blog
prev: blog/
sidebar:
  open: true
math: true
---
<figure>
  <a href="https://www.vim.org/" target="_blank">
  <img src="/images/vimlogo.png" width=20%>
  </a>
</figure>

## TLDR

Visual Improved is a console text editor known for its efficiency and powerful keyboard-centric approach.
  - Veteran: Improved version of the classic "vi" editor, ubiquitous in Unix systems.
  - Keyboard Maestro: Highly customizable and thrives on keyboard commands, ditching the mouse for speed.
  - Steep Slope: Learning curve can be brutal, but mastery grants impressive editing speed and navigation.

## Introduction

I was introduced to Vim out of necessity rather than curiosity. In the software engineering world it is considered an essential skill as some of the key courses demand the use of a a remote Linux cluster.

[CSSE2310](https://my.uq.edu.au/programs-courses/course.html?course_code=CSSE2310) is a computer science course at UQ that really introduces one to software engineering. It covers 3 areas: 
  - **Writing C code** from scratch,
  - The use of **Linux Shell, Vim, and Tmux**
  - **General computer systems principles** such as processes, threads, memory allocation, filesystem essentials, memory virtualisation and computer networking. 

If you are familiar with any of the above-mentioned concepts, you can probably already tell that this course demands countless hours reading through the `man` pages and hair pulling at compilation errors and tracking down memory leaks, especially for someone fairly green in the field. Needless to say, when I, a mechanical engineer by education and rookie Python scripter by trade, signed up for it, I didn't have a clue about what any of those were.

By then I had only really used Linux briefly in a [Computational Fluid Dynamics](https://my.uq.edu.au/programs-courses/course.html?course_code=MECH6480) (CFD) course, where it was possible to get through the course by simply following along at tutorials and using online resources, without actually learning much about Linux.

## Trial by Fire

My first encounter with Vim felt akin to being thrown into the deep end of a pool without knowing how to swim. The cryptic commands, the seemingly arbitrary key combinations—everything about Vim was intimidating. Yet, as I delved deeper into CSSE2310 and the world of software engineering, I realized that Vim was not just another text editor; it was a tool forged in the fires of efficiency and productivity.

With each passing day, I forced myself to embrace Vim's keyboard-centric approach. I stumbled through the basics: navigating the cursor, entering insert mode, and executing simple edits. Every mistake felt like a setback, every command a triumph. But slowly, gradually, Vim began to reveal its secrets to me. I learned about modes, registers, and commands like :wq that felt like incantations from a wizard's spellbook.

## Finding my Vim Mojo: Embracing the Motions and Customisation

Discovering the transformative potential of Vim's motion commands was a pivotal moment in my journey. Initially intimidating, these commands soon became my trusted companions, enabling me to navigate my documents with unparalleled precision and efficiency. With practice, I harnessed the power of customization, crafting shortcuts tailored to my workflow. Each shortcut felt like reclaiming a piece of control over my editing experience, transforming Vim from a mere text editor into a personalized tool that anticipated my every move.

## Holy NeoVim 

Doing lots of mechanical engineering work at the time which requires the use of Windows-based CAD modelling packages (Solidworks nad NX), I decided to install the NeoVim on my Windows laptop.

Just when I thought I was getting the hang of Vim, I stumbled upon NeoVim -- a modernized, enhanced version of the classic editor. Initially I was reluctant, because I did not understand the requirements of a Windows based customisation, but the allure of NeoVim's modern features and improved performance proved too tempting to resist. A few tutorials and blog posts later I successfully called `:PlugInstall` and with that I began my exploration of the Nvim plugin universe.

## Vim \& LaTeX

After a few months into my Vim Journey I have decided to update my LaTeX resume and opened [Overleaf](https://overleaf.com). Immediately I felt like something was wrong. My key-bindings didn't work. I began investingating the my vim-plug options and syntax highlighting plugins such as [VimTeX](https://github.com/lervag/vimtex) and seamless integration with LaTeX compilers like [MikTex](https://miktex.org/) or [TexLive](https://www.tug.org/texlive/), Vim transformed the way I approached writing technical documents. 

Whether it's navigating to a specific line, jumping to the next occurrence of a word, or selecting a block of text with surgical precision, Vim's motions empower you to navigate any document with unparalleled speed and accuracy. 

Consider, for example, the simple act of navigating through a large LaTeX document. In a conventional editor, you might find yourself endlessly scrolling or tediously clicking through menus to find the section you're looking for. But with Vim, a few keystrokes are all it takes to zip effortlessly from one section to the next, thanks to commands like `/{pattern}` and `[[`.

## The Vim Journey Continues

My journey with Vim is far from over. As I continue to explore its myriad features and expand my proficiency, I am constantly amazed by its depth and versatility. Each day brings new challenges and discoveries, whether it's mastering advanced editing techniques, customizing my workflow with plugins, or integrating Vim into other aspects of my work.

## Resource Links

If you're an experienced Vim connoisseur or a rookie, you will have your config pretty finely tuned, but just to feed your curiosity, below is my personal config link and some other resources, for those who haven't delved into the world of overoptimisation of their terminal tools.

{{< icon "github" >}}
[My Vim Config Repo](https://github.com/borslap/vim-conf): My personalized Vim configuration development was incubated in Windows version of NeoVim, which locked me into Vim script or `init.vim` instead of Lua-LaTeX to configure it. Since migrating onto Linux I have started the migration to Lua.

{{< icon "github" >}}
[NeoVim Kickstarter](https://github.com/nvim-lua/kickstart.nvim): Get started with this guidance-packed Vim config repository, led by the developer community or contribute to the future of text editing!

{{< icon "github" >}}
[NV Chad](https://github.com/NvChad/NvChad): One of the more hyped battery-included Vim plugin configurations on the internet. I think it's over-plugged, but if you take a few things out, it's not too hard to make it work for you.

{{< icon "link" >}} [Vim subreddit](https://www.reddit.com/r/vim/): Join the vibrant Vim community on Reddit to share your expertise (or lack thereof) or just to crack jokes. Connect with fellow Vim enthusiasts from around the world.

