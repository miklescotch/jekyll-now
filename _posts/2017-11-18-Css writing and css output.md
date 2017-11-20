---
published: true
---
> Two differincies (Russian fun sentence)

Ok. Let me start about this.
Let me assume we have some tag container - i'll change syntax a little bit for my needs

`<div - div />`

so we have this div
let's start to change it's initial css
of course we can and would do this on Sketch by adding all style inside element 
but in our world we need to use classes - shorthands for styles - yeah it;s just a shorthand with id
so
it would look like this
```
morphling :details
	tag: div - means something (symbols:3)
    parent: body - means something
    etc: means something
	position-styles-CLASSNAME
    common styles-CLASSNAME2
    unique styles-CLASSNAME3
    javascript styles-CLASSNAME4
```

```
<div class="lt cb avatar avatar_blue j-clickable"></div>
lt - left top
cb - color blue
```
    
This is common idea.
Lets think about it other way.
It was humanible logical naming and bunching.

But anyway it's just a stuff of text - in the end. Only human mind divides it on logical parts.

So what we can is have some help-transpiler.

This friend of us will help thus:

``<div class="lt cb avatar j-c"></div>``

transpile into

`<div class="avatar-lt-cb-jc"></div>`

Why so?

cause first i thought - wow let's have special selectors in use such as:
	
    *[-lt-] { snippet }
    
    *[-cs-] { snippet }
    
Well bad idea jeans - they are too specific
So?

Lets have unique class all in one - which would have all of this stuff inside.

That is where this term comes to help - 2 editions workflow.

What does it mean - well, 
1edit. you are working with unity library and name dom elements with a BEM (or whatever) - and transpile it to BEM+unitycss names and selectors (html and css)
2edit. You add all human mistakes and non-systematic features to your css generated selector like .avatar_lccbjcbgr (here we have 2 parts - humanreadable and just a abracadabra (for css) - so we have both methods.)

You shouldn't worry about constantly changing your @unitycss@ - it works forever and ever. But you have genereated classname - which is unique - so you just add your @exceptional styles@.

So you have
unity css as little as possible (lt, cb, bgg, jc. dn)
+
BEM naming for kind a readable part
= generated unique class 
and + 2 edition adding (exceptional styles for unique class)

and that is all.
If you would need remove or change something - you should decide where? unity? bem? or exceptions?
no need for long BEM mod names, no need to worry for resystemize general unitycss. just 2 editions workflow.