---
layout: single
title: "Markdown Programming Language"
date: 2025-03-21
author: Ayush Kanodia
categories: markdown programming
usemathjax: true
author_profile: true
toc: true
---

# Is Markdown the new programming language?

I've been building with an AI programming agent (I use Cursor). I love using it. Every time it achieves something it couldn't before, I feel delight, followed by an absurd feeling of almost throwing up because I cannot imagine the upper limit of where this is going, and some existential worry around the value of the skills I've been trained for.

However, sadly but somewhat relievingly, it is not good at making very large code changes. Perhaps this is because my prompts did not specify enough; perhaps because the underlying model is not good enough. Which of these two is the case is interesting, but is not the point of this writing.

In order to avoid a code blast and then having to painfully go through/fix it, I've been planning out a large code change in markdown first. Of course, I've been doing this in Cursor, with the agent's help. The goal is to break it down enough such that I have faith that each individual step is something I clearly understand and can test, as well as trust that Cursor will easily implement it.

In doing so, I came to hate the fact that I'm not actually 'programming', and was 'wasting my time' writing markdown. In sulking about it to myself and my wife, I told myself that this is something that well paid PMs etc do all the time - so it must be real work. Then I connected this to the thought that prompting feels like the new programming language, and LLMs just the new compilers, except that they have this weird probabilistic nature of messing up really badly once in a while. 

So what is the new language? My thoughts go towards better natural languages like Sanskrit/Esperanto (I don't know which ones are best). But also it's not just about language. Structure beyond language will matter too. And now I'm allowing myself to think Markdown is a strict improvement to 'vanilla' text, and is my current programming language, at least as measured by how much time I spend in it. It has lots of extra structure and information. 

At the very least, I now feel like a programmer when writing Markdown. That's a win.


PS: I come from org mode in Emacs, which doesn't have much Cursor support. After getting used to folding in Markdown, I feel it's pretty similar. I struggled a bit with making the `j` (line down) motion in vim mode not open a fold by default until I realized that in Cursor/VSCode this is an actual line down and can be easily mapped to `gj` which is screen line down. I most liked orgmode for its tab-based folding. I feel stupid that I did not use Markdown similarly before.

Edit (4/3/25): I do not think [natural language has the precision required to specify precisely](https://www.cs.utexas.edu/~EWD/transcriptions/EWD06xx/EWD667.html), but that we are moving from something low level (now python) to something higher level ideal for LLMs, which is more precise than Natural Language. .