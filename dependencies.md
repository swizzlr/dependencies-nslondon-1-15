# The Dependencies You Didn't Know You Had
^
- Good evening
- Name a dependency
- This talk asks that you expand your notion of a dependency beyond AFNetworking and ReactiveCocoa
- But let's get something straight: a dependency is a necessity for your project. But to other people

--- 

1. a thing

^At worst a dependency is

----

1. a thing
2. that you have to support

--- 

1. a thing
2. that you have to support
3. and unless you pay money nobody will help you

---

1. a thing

^At best a dependency is

--- 

1. a thing
2. that someone else maintains for free and for which help is generously given for free

^Emphasise that, be nice to open source contributors

--- 

1. a thing
2. that someone else maintains for free and with which help is generously given for free
3. that makes your life easier

--- 

##Code specific knowledge (aka legacy code)
> "No, we don't ever push view controllers. There are methods on the root view controller that present and hide for us. Use the enum to specify how you want to present the view controllers."    

^
- When you diverge from the standard libraries, you ask more of your programmers

--- 

##Code specific knowledge (aka legacy code)
> "Call the `FacebookHandler`. Except for login. Yeah, don't use that method."

^
- If something is deprecated or misnamed, document it (ideally with the compiler)

---

##Conceptual knowledge (aka "Why Does Your JSON Parsing Look Like Hieroglyphs?")
> "It's easy, you just have to know where to bind your monad to the right function."

^
- Foundation, AppKit and UIKit are lightly OO and procedural frameworks
- Nowhere in the Objective-C or Cocoa programming guides do the words "functor, applicative or monad" occur

---

##Conceptual knowledge (aka "Why Does Your JSON Parsing Look Like Hieroglyphs?")
> "It's easy, you just have to call `getObject:` on the provided factory and then pass it into the initializer as a configuration object before passing it on to the final network request in the graph."

^
- Neither is it Java!

---

##Tool specific knowledge (aka "Why Did Nokogiri Fail To Compile?")
> "Have you tried using RVM?"

^
- Joel Test recommends a one step build process
- `script/cibuild` should be your oneliner to unit test happiness, and possibly an IPA
- We are not Ruby developers, we are Objective-C and Swift developers. Bash is the lingua franca of Unix
- Bundle/carthage as part of your daily routine is an antipattern

---

##Tool specific knowledge (aka "Why Did Nokogiri Fail To Compile?")
> "Did you `git reset --hard`? Oh, wait, you tried to add a submodule? `git rm`, I think. Shoot, `rm -rf`. Huh?"

^
- This cuts both ways. Even the "official" tools suck. Beware of the complexity inherent in powerful tools

---

##Culture specific knowledge
> "🔥"

^
- Github talked about this the other day
- Textual communication is hard, and depends on social culture and company culture

---

##Culture specific knowledge
> "You reverted my PR!"

^
- Have a contributing document explaining what's expected

---

#DON'T PANIC!

^
- We all have these dependencies, and we need them
- I'm not telling you not to do any of these things
- I'm asking you to evaluate your 
	- culture
	- tools
	- paradigms
	- headers
- So onboarding is easier, your replacement likes you, and it's easier to move with new apple technologies

---

#Thanks to Ash Furrow for his feedback

---

#Thanks to my wife Lisa for making me do this

---

#Thanks to you all for listening

##Twitter, Github: @swizzlr
##Email: me@swizzlr.co