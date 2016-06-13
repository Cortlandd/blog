---
title: My Plans for Using Haskell
---

## Warning: I go on a tangent sometimes and I suck at wording things. I'm sorry. One of many things about myself I need to work on.

"So why do you wanna write haskell kid? You talk alot of big shit on twitter about languages you dislike and how much you enjoy haskell. What do you want out of programming? Whats your story you little shit?"

So everyone has their reason for using a certain programming language. Majority of people will say "I use whats best for the job". yeah...must be nice. I just think Haskell is fun.

I started learning Haskell consistently about 2 1/2 months ago. I skimmed through some Haskell code months previous and accused it of being the anti-christ language and that people who write it aren't human. I still feel that way about people who write C++. Thats a post for another day. A small snippet came across my screen one day and I said "fuck it, let me google 'try haskell' and see what happens". After a run through tryhaskell and a bit of research into Functional Programming I decided this was for me. With Haskell you're very explicit on what you want your program to do. List comprehension is what sold me. Not sure why, but something sticked.

specifically:

```haskell
> [ x * 2 | x <- [1..10] ]
	
[2,4,6,8,10,12,14,16,18,20]
```

Yes in Ruby I could write:
but haskell has personality. personality goes a long way.

```ruby
(1..10).map { |x| x * 2 }
```

My goal when I get more comfortable with Haskell, doing so using HaskellBook, my two professors Julie Moronuki & Chris Allen, the homie Gabe @ haskellforall.com, and the geniuses (I say this literally. The people in this community are smart SOBs) behind many big pieces of haskell, I'd like to make any good contribution I can. Rather is a tutorial, bug via github, etc.

I look at Haskell like a puzzle. You gather all the separate puzzle pieces (functions), and connect them together (higher order functions, etc). And after connecting many pieces, they all line up for the intended image result. Well...that's if the compiler agrees (see what I did there?).

again, sorry I suck at wording things, and grammar, punctuation, etc. there is a reason i like math.
