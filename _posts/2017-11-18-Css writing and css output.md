---
published: true
---
> Two differincies (Russian fun sentence)

Ok. Let me start about this.
Let me assume we have some tag container - i'll change syntax a little bit for my needs

<div - div />

so we have this div
let's start to change it's initial css
of course we can and would do this on Sketch by adding all style inside element 
but in our world we need to use classes - shorthands for styles - yeah it;s just a shorthand with id
so
it would look like this
morphling :details
	tag: div - means something (symbols:3)
    parent: body - means something
    etc: means something
	position-styles-CLASSNAME
    common styles-CLASSNAME2
    unique styles-CLASSNAME3
    javascript styles-CLASSNAME4

	<div class="lt cb avatar avatar_blue j-clickable"></div>
    lt - left top
    cb - color blue
    
This is common idea.
Lets think about it other way.
It was humanible logical naming and bunching.

But anyway it's just a stuff of text - in the end. Only human mind divides it on logical parts.

So what we can is have some help-transpiler.

This friend of us will help thus:

	<div class="lt cb avatar j-c"></div>

transpile into

	<div class="avatar-lt-cb-jc"></div>

Why so?

cause first i thought - wow let's have special selectors in use such as:
	
    *[-lt-] { snippet }
    
    *[-cs-] { snippet }
    
Well bad idea jeans - they are too specific
So?

Lets have unique class all in one - which would have all of this stuff inside.
