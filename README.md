# How to Code

There are cooks and there are chefs. A cook is someone who can follow a recipe. They pick up a recipe book, read it, and make something wonderful. A chef is someone who can make new recipes. They understand their ingredients. They know what goes with what.

New coders often talk about being stuck in tutorial hell. They watch a video which shows them step-by-step how to build a Twitter clone with React. They read recipe after recipe, but they never come to terms with the substrate. They know a bunch of things that work, but they don't know why. They are cooks, not chefs.

In this book, I'm going to help you become a chef. This will be easier than you think, because once you understand the fundamentals, code isn't that hard.

A food chef has hundreds of ingredients to pick from. They must understand chemistry, the action of heat, the interaction of flavour molecules. A code chef has a much simpler time. We have only seven basic ingredients to choose from that we can slot together in a variety of ways to create whatever you want. 

## Seven Fundamental Ingredients

The fundamental ingredients of code are:

* Values: Things that you can use
* Variables and Arrays: Places to put those things
* Expressions: Convert values into other values
* Loops: Do the same thing over and over as many times as you like
* Conditionals: Do something if something else is true
* Functions: Pass values to a thing and expect a result
* Objects: Bundle variables and functions together into logical groups
* Classes: Things that can help make objects

That's it, that's all there is. Every device you have ever touched is made out of these parts. These are the lego bricks in your big box of lego. They are your minecraft blocks. This are all you get. The challenge is working out how to put them together to do what you want them to do.

You can learn these blocks in a couple of evenings, but mastering how they fit together takes lifetimes.

# Why you want to read this book

In the first part of this book, I'll teach you all eight basic building blocks of code. Once you know these, you'll be able to apply them to any language.

In the second part of this book, we'll look at patterns

# Because being a Software Engineer is Awesome!

And being a Software Developer is amazing. I have a friend who lived like a king in a Spanish village for ten years on a London salary. People travel, they work from a laptop, they buy a big house and live comfortably with their family. Anyone can try to do it. Code doesn't care if you're young, old, black, white, male, female. It doesn't really care if you have a degree. You either can code, or you can't, and if you can code there are people out there who will pay you well to do it.

# What is a computer

This is a computer. This is Babbages Difference Engine, designed by Charles Babbage in 1849 but not completed until 2002. It has 675 bytes of data and runs using a hand crank, which gives it a top speed of roughly one hertz.

This is a computer. This is the first IBM PC, released in 1981. It has 16K of RAM and runs at 4.7MHz, that's 4.5 million times faster than the Difference Engine.

// TODO: Check these facts

This is a computer. This is an iPhone XS Max, released in 2018. It has 4Gb of RAM and a clock speed of 4x1.6GHz. If you wanted to run iOS on the Difference Engine, the memory would need to be the size of North America, and the handle would have to turn faster than the speed of light.

These machines look very different, but inside, they're all fundamentally the same. They have memory, and they have a processor. The processor picks a number, works out what to do, then picks the next number, works out what to do, and the next, and the next, until the process is complete.

We represent computer memory as a big list of numbers. In Babbage's case, just 675 numbers can be stored. In the iPhone, you can store 4 billion numbers in working memory. Imagine a line of 4 billion numbers stretching into the distance. Each number has a location, we call it an address. At address one, we might find the number five. At address one million we might find the number twelve.

When we want the machine to run a program, we give it the address of the start of that program. The CPU then gets the number from that location. Say it gets a five. The CPU has a list of things it can do, so it looks on that lst for number five. That



## Variables

We can think of computer memory as a great long line of numbers stretching off into the distance. If we wrote those numbers out on paper, an iPhone X with 4Gb of RAM would go right around the world.

Every location is identified with an address. If our program wants to get the number stored at position 45, it asks for that memory address, and the computer memory dutifully replies. This is a problem.

Modern computers run lots of programs at once. If I can write a program that can write to arbitrary memory locations, then what's to stop me reading the data from other programs that are running on the machine? What's to stop me from changing them? I could rewrite another program's data while it was running. I could rewrite its code.

Imagine I'm running a program and I can't necessarily know that some other program isn't going to come and wreck my stuff up. It would be complete anarchy, a single programming mistake could take down the entire operating system. This is how computers used to be. There is a type of hack called a buffer overflow, when you read from your own memory until you reach the end, and then suddenly you're reading from something else's memory.

Nowadays programs have to request memory from the operating system. In a language like C you do this explicitly:

    malloc(15);

Gets you the location of 15 bytes of memory that you can use for whatever you like. You then have to be careful to only write to that location and free it once you're done. As you can imagine, this is hugely powerful, but also hard to manage. Ideally we want to abstract away this explicit memory management. We could let the computer handle putting data into the memory, and then refer to that data using a handy, human readable word.

And this is a variable.

I can write

   numberOfCats = 12

This says:

1. Give me a memory address that I can write to
2. Write the numeber 12 to that address




