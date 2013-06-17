# Web Development Basics

## Intro

Now that you know what web developers do, it's time to start thinking about how they actually do it.  In this unit, we'll learn about how the Web works and start thinking about the basics of computer and web programming.  You can consider this the "Prep Work" section of this curriculum but it will also serve as a reference for later.

Each of the following sections represents essential baseline knowledge.  Even if you have no intention of becoming a web developer yourself, this material should help you gain a useful understanding of the moving parts involved in creating and serving content on the web.  We will start by familiarizing you with the internet and your own computer.  You will then learn the basics of front end technologies like HTML, CSS, and Javascript before stepping into the back end with a brief foray into Ruby and Ruby on Rails.  We will finish by learning about databases and topics like git workflows and software in the cloud.  

By the end of this unit, you should not only understand how the web works, but be able to identify and differentiate each of the technologies that you will be learning in order to build web applications of your own.  You will be able to build a simple webpage, style it, and add minor elements of interactivity while working comfortably from the command line.

We will cover a very broad swathe of knowledge here and that's intentional... it's silly to go diving straight into server-side programming without having a context for what it is and why it's useful (and why you should learn it!).  Each section will contain questions that you'd better be able to answer before moving on.  For the first time, some of the sections below will ask you to do exercises to help build your understanding.  Give it a shot!

## How Does the Web Work?

##### You will need to understand:
* What is the internet?
* How is information broken down and sent?
* What are packets?
* What is a "client"?
* What is a "server"?
* What is HTTP and how does an HTTP request work?
* What are DNS servers?
* What is HTML and how is it used?
* What is CSS and how is it used?
* What's the difference between static and dynamic web pages?
* What happens when you click "search" on google.com?


Check out [How Does the Internet Work? (video)](http://www.youtube.com/watch?v=oj7A2YDgIWE) for a basic explanation of how packets work.

Harvard's David Malan explains internet basics starting at 52:15 in [this lecture](http://cs50.tv/2012/fall/lectures/7/week7m-720p.mp4) from their popular Intro to Computer Programming course.  Pay attention to opening the developer tools he talks about around minute 58... you'll use that a lot.  We'll get heavily into HTML later in this curriculum.

He dives further into HTTP in a [short 3-minute video (video)](http://cs50.tv/2012/fall/shorts/http/http-720p.mp4).

For a more detailed (though dated) text explanation, [check out this link](http://www.garshol.priv.no/download/text/http-tut.html).

What's the best explanation of how the web works you've seen or read?  Were any other resources you found to helpful for answering the questions posed at the beginning of this section? [Let us know!](mailto:curriculum@theodinproject.com)

#### Additional Resources:
* [A packet's journey (video)](http://www.youtube.com/watch?v=WwyJGzZmBe8).
* An [entertaining TED talk](http://www.ted.com/talks/jonathan_zittrain_the_web_is_a_random_act_of_kindness.html) about how the Internet works.
* How the web works... [a cartoon](http://landofthefreeish.com/pics/how-the-internet-works/).
* Udacity has a quick explanation of [web basics](https://www.udacity.com/course/viewer#!/c-cs253/l-48737165/e-48230539/m-48742046) and [HTML basics](https://www.udacity.com/course/viewer#!/c-cs253/l-48737165/m-48724340) (these will require login/signup but it's free).
* A comprehensive list of web development resources lives at the [Web Standards Curriculum](http://www.w3.org/wiki/Web_Standards_Curriculum).


## Step Back... How Does Your Computer Work?

This isn't a course about rebuilding your hard drive but it is useful for you to understand the high level overview of what's going on to make your computer function.  That's partly because you'll see the same patterns showing up when you're telling servers what to do and partly because you're going to have to talk to your computer in a way that it understands anyway so you'd better speak a little of its language.

Spare 15 minutes to [learn how computers work](http://www.youtube.com/watch?v=WIDzNyfVVg0).

### The Command Line

Raise your hand if you're scared of the command line.  Yes, we have this image of developers staring at a black screen with white or green text flashing across while they wildly enter incomprehensible commands and hack into the corporate mainframe (spilling soda and wiping cheetos off their keyboard no doubt as well).  

That black screen (or window) is the command line, where you're able to enter commands that your computer will run for you.  And while that image of a programmer is a bit overdone, the command line really is sort of like our base of operations, from which we'll launch other programs to do our "real developing" in.  It has a syntax of its own which is different but not all that difficult to pick up.  You'll be entering the same commands dozens of times anyway, so you'll get pretty good at it in a short period of time.

To gain a better understanding of your command line, take this [Command Line Crash Course](http://cli.learncodethehardway.org/book/) by Zed Shaw.

## Terms to Know

Take a look at this [list of term definitions](http://prework.flatironschool.com/#terms) and make sure you have at least a competant understanding of each one (click on it to bring up the full definition).  Don't skip this and assume you know it all -- there will be at least a few that are worth nailing down.  Flashcards help.

## Web Programming 101

Many of the things we're about to cover will be handled in much greater depth later on in the curriculum but it's important to get a basic level understanding of what they are and how they're used so you can still see the bigger picture while you're down in the weeds learning that stuff.  Take the time to get to know each of the major building blocks of a web application, from the front end to the back end and into databases.  And just because we're covering a lot of material doesn't mean we're not learning anything well -- you'll be spending a good bit of time becoming familiar with the "101" level of each technology.

### Front End 101

The "front end languages" live in the browser.  After you type in an address in the address bar at the top and hit Enter, your browser will receive at least an HTML file from the web server.  That file will likely tell the browser to go and also ask for a CSS file and a Javascript file as well.  Each of these languages performs a separate but very important function and they work harmoniously together to determine what the web page IS, how it LOOKS, and how it FUNCTIONS.  And keep in mind that your BROWSER handles figuring out how to make these files into a functioning webpage (not the server).

Get a high level overview of how all three languages (and jQuery) work together in a web page in this brief learn.jquery.com post on the [Anatomy of a Web Page](http://learn.jquery.com/javascript-101/getting-started/).

#### HTML and CSS 101

##### You Will Need To Understand (at least):
* Why do we separate HTML and CSS?
* What are classes and IDs (and how are they different)?
* What are elements?
* What are tags?
* What are attributes?
* What are forms?
* What is a div?
* What are selectors?
* What are properties?
* What are values?

As you've hopefully [learned before](http://www.skillcrush.com/terms/html.html), HTML is the markup that contains all the actual stuff that a web page has.  All the text on this page lives inside HTML tags that tell your browser how to order the content on the page.  [CSS](http://www.skillcrush.com/terms/css.html) tells the browser if you want to display any of those tags a particular way like, for instance, turning its background blue and pushing it a little to the left.

Do the [Codecademy HTML/CSS track](http://www.codecademy.com/tracks/web) for a healthy baseline understanding of HTML and CSS.

##### Mini-Project



##### Additional Resources

Watch all the [free HTML videos](http://teamtreehouse.com/library/websites/html/introduction) from Treehouse and take the quiz. 

Check out the [quickie CSS introduction](http://teamtreehouse.com/library/websites/build-a-simple-website/website-basics/introduction-to-css) from the same people as well.

If you want to see the art of CSS, check out the [CSS Zen Garden](http://www.csszengarden.com/), which collects submissions that use identical HTML and modify only the CSS but turn out wildly different (and beautiful).

Read through [Shay Howe's HTML&CSS Tutorial](http://learn.shayhowe.com/html-css/terminology-syntax-intro).  Lesson 1 gives a solid overview and you can do the whole thing for a more in-depth understanding.


#### Javascript and jQuery 101

##### You Will Need To Understand:
* What is a scripting language?
* What is a variable?
* What is the DOM?
* How can you interact with the DOM?
* What are events?

As we [saw before](http://www.skillcrush.com/terms/javascript.html), Javascript is the in-browser code that gets run to make things on your webpage moveable and clickable.  It's time to dive in a bit more and start getting your hands dirty with some code. 

Do [Codecademy's Javascript Section 1](http://www.codecademy.com/tracks/javascript)("Getting Started with Programming" and the accompanying project).  If you want extra credit, do the full Javascript track... but we'll get to that in-depth later on in the curriculum.

What about [jQuery](http://skillcrush.com/2012/07/23/jquery/)? It's a library of commonly used javascript widgets and functions that more or less has taken the internet by storm.  It's actually written in javascript so you don't have to go through the pain of writing out, for instance, a popup modal dialog box the long way.  It also gives you the incredibly easy ability to select elements on the webpage ("DOM elements") so you can start modifying their properties.

Learn about jQuery by doing [Codecademy's jQuery Section 1](http://www.codecademy.com/tracks/jquery)("Introducing jQuery") and [Code School's try jQuery](http://try.jquery.com/).  The remaining Codecademy sections are, again, extra credit and will be covered later in the curriculum.

##### Additional Resources

Reading: The first several sections of the [Javascript 101 tutorial on learn.jquery.com](http://learn.jquery.com/javascript-101/).

Interactive: Do the additional sections in the [Codeacademy Javascript Track](http://www.codecademy.com/tracks/javascript).


##### Mini-Project


### Back End 101

The three languages of the front end are fairly standardized -- HTML for presentation, CSS for markup, and Javascript for scripting.  The back end is a different story... you can run pretty much anything you want to on your server since it doesn't rely on you user's browser understanding what's going on.  All the browser cares about is whether you've sent it properly formatted HTML, CSS and Javascript files (and other assets like images, videos, etc.).  That's led to a whole lot of different choices for back-end languages.  As long as it can take in an HTTP request and spit out some HTML, you can probably put it on a server somehow.

That said, some languages are more popular and practical than others.  If you're running your own server, you have a ton of flexibility but plenty of headaches.  If you're deploying to the cloud (which we will be doing later), you may be restricted to those languages which your cloud provider has installed on their platform... it doesn't do you much good if the servers you're "borrowing" from them can't understand your code!  Some of the most popular are PHP, ASP.NET, Ruby, Python and Java (not to be confused with Javascript).  And just like I can say "which way to the nearest pub?" in German, French, Italian, English and Bad English, all of those languages can perform almost exactly the same functions.

#### Ruby 101

##### You Will Need to Understand:
* What is an "interpreted" language?
* What is IRB?
* What are Objects?
* What are Methods?
* What are Classes?
* What are Blocks?
* What is an Array?
* What is an Iterator?
* What are hashes?
* What is a lambda?
* What is a proc?
* What is a library?
* What is a gem?


Our focus will be on Ruby, the language designed for programmer happiness.  What takes a hundred lines of code in Java could take just a couple in Ruby because it prepackages lots of sneaky functions into easy-to-use convenience methods.  It has occasionally been critisized for not running as fast as some of the other languages, but that's not so much an issue when you can just load more servers/instances.  The benefits of being able to write code much faster and with less headache allow you to iterate much faster when building a website and so the end product is more likely to suit the client or the user's needs.

It should be said that Ruby's "twin" language is Python.  In some ways, they sort of resemble romance languages -- once you've learned one, it's not terribly hard to pick up another because they tend to follow many of the same conventions, just using different "words".  Python tends to be taught more in colleges and is used a fair bit for more data-intensive applications.  But Ruby has a secret weapon that makes it the love of fast-iterating website production -- the framework Ruby on Rails (which we'll cover in the next section on Frameworks).

With either of the languages, there are a couple of things that aren't immediately intuitive but become very useful when you understand them.  We'll do an introduction to Ruby here and then, in the unit on Ruby, you'll get to understand it like the back of your hand.

First, go to [tryruby.org](http://tryruby.org) and do the quick exercises there to get your feet wet.

Next, read through the [Ruby in 100 Minutes](http://tutorials.jumpstartlab.com/projects/ruby_in_100_minutes.html) project from Jumpstart Labs.  If you can't get IRB running, check out the [Installation Unit](/installations) to get everything up and running or, if you'd rather wait, just try to follow along.

Dive in a little deeper with Chris Pine's [Learn to Program](http://pine.fm/LearnToProgram/?Chapter=00).  Try to do the exercises at the end of each chapter.  Take a crack at chapter 10, but don't feel disheartened if it still doesn't click for you.

Finally, conquer the [Ruby Monk's Introduction to Ruby](http://rubymonk.com/learning/books/1).  If you're shaky on Hashes, Blocks, Procs, Lambdas, Modules, and I/O... you're not the first and won't be the last so have no fear.  We'll dive deeply into those in the coming units.

##### Additional Resources

The Railsbridge [Ruby Language](http://curriculum.railsbridge.org/curriculum/ruby_language) unit.

Textbook: Peter Cooper's [Beginning Ruby](http://www.amazon.com/books/dp/1590597664) chapters 1-8 will cover the material in greater depth than you really need to here but may help you shore up some of the concepts.

### Frameworks 101

#### You'll Need to Know:
* What is a framework?
* What languages have frameworks?
* What is open source software?
* What is MVC?

If you're programming with Ruby or any other language, you pretty much start with a blank file and go from there.  Programmers, the best of whom are pretty lazy folk, got tired of having to write the same code over and over and over again just to cover the basic tasks that they wanted their applications to perform.  So they batched that recycled code together so they could start off a new project without having to do all that work again and called it a framework.

Another benefit of using a framework is organization.  They tend to force you to organize your files and code in a way that keeps it highly modular and really clean.  When you start a new Rails application, you're given dozens of folders already organized in a heirarchy which makes sense and follows good Model-View-Controller (MVC) separation principles.  It's not quite "color-by-numbers" for code but it certainly keeps things ordered.

There are often several different popular frameworks for a given language.  They can have exciting names like Ember, Meteor, Django, Rails, Grok, etc.  Wikipedia has a [comprehensive comparison of frameworks](http://en.wikipedia.org/wiki/Comparison_of_web_application_frameworks) that should give you an appreciation for the number of them.

A final thing to note is about licensing -- frameworks are typically open-source and their license allows you to use them, modify them, make money off them, sell products with them etc. all without owing any fees to their original creators.  You may not think too much about that as you blithely code away using other people's frameworks, but it's a very important distinction between open-source frameworks and commercially produced/sold software.  We'll get more into Open Source Software (OSS) in later units.

#### Ruby on Rails 101

You're probably here because you want to learn Ruby on Rails but you may not be entirely sure what it is.  Well, Rails is just a bunch of ruby code written to handle the parts of a web application that you don't often want to think about.  Rails uses, as you'll often hear, "convention over configuration".  That means that Rails has made a lot of decisions for you about how things should be structured and how the code should run.  You can change them, but it's best if you just go with the flow and work within their rules (especially as a noob).  

Think of it like buying a suit -- you probably don't care where the thread was sourced, which hands pulled the loom, which companies shipped the fabric, how the lining is mated to the jacket, what sorts of buttons are on there... you trust the tailor to have figured all that out and you just want to be able to buy the nice looking grey one in size 42 regular.  

As you saw in the introduction:
>>Why Rails?  Why not.  There are dozens of possible technologies out there to choose from and, frankly, they do pretty much the same things.  Rails is attractive because it's a relatively straightforward and very well documented framework that's used by tons of great startups and tech companies today and it has a very strong community of developers and students who support it.  It lets you put up a functioning website in hours not days or weeks.  The "in" tech will probably be something completely different in a few years, as it always is, but Rails presents a great platform on which to build the skills you need to carry you to that next phase.

Because Rails has made a lot of decisions for you, you can work incredibly fast.  You can have a website up on the internet (though it won't look like much) within a couple minutes.  The very first time you generate a new project, everything is in place so you just have to fire up your local server (by typing simply $ rails s) and you'll already see the Rails welcome page up there.  Then it's just a matter of plugging in all the pieces you actually need to make your rich web application run.  It also means that you can start immediately making small changes and seeing how they affect your application where before you would have had to build a ton of infrastructure and write lots of code before seeing a single thing change live.  Rails makes your life a whole lot easier!

Rails also firmly organizes your code using an MVC pattern which you will come to know and love.

#### Backbone.js 101

You thought only server-side languages could utilize frameworks?  Think again.  More and more heavy lifting is being done in the browser these days and that means lots of repetitive and disorganized code to tidy up.  While there are many popular Javascript framworks, we'll focus on Backbone for the same reason we're focusing on Rails... it's probably the most straightforward and best documented one out there.  That doesn't mean it's the shiniest or the newest, but if you've mastered your fundamentals in Backbone you'll be more than capable of picking up a slightly more esoteric framework.  And there are a whole lot of websites out there that need to be built and maintained in Backbone (ahem, jobs).

### Databases 101

#### You should know:
* What is a database?
* What are relational databases?
* How are relational databases different from XML?
* What is SQL?
* What does CRUD stand for?
* Why is CRUD so important for web apps?

We've talked about the client-side and the server-side, but how do we keep ahold of all our user's data?  Who remembers that your login password is CatLover1985 so you can sign into the website?  The bottom layer of any web application is the database and it handles all the remembering for you (we'll cover caching much later).  It can be relatively simple, like an excel spreadsheet, or incredibly complex and split into many giant pieces like Facebook's.  

Databases are one of those aspects of web programming that are kind of hidden in the back and so people treat them with a sort of suspicion and awe.  That's nonsense and you should get over it -- your database and you are going to become very good friends (or frenemies).  By the end of this curriculum, you're going to understand what's going on with your databases and be able to interact with them like a pro (and probably better than some people you'll work with).  

Compared to a normal language, SQL (Structured Query Language), which is used to query databases, is a very simple syntax... there are only a small handful of verbs to learn.  What trips people up is that you need to be able to visualize in your head what it's going to be doing.  We'll spend a fair bit of time on SQL and databases because they're so fundamental, but for now we'll just cover enough to get you familiar with what's going on:

A pretty good plain-english explanation of SQL can be found from Zed Shaw at [Learn SQL The Hard Way](http://sql.learncodethehardway.org/book/introduction.html).

Sign up for Coursera's [Intro to Databases](https://class.coursera.org/db/lecture/index) course and watch the lectures on Relational Databases and SQL (~3 hrs).  You can save the sections in between (relational algebra, XML, JSON) for extra credit (things get a bit technical there).

Do the [Automated Assignments](https://class.coursera.org/db/quiz/index) for the SQL section to get a jump on your understanding for the SQL unit we'll be doing later.  Try working with a pen and paper next to you to draw pictures of what's going on.  Again, you can save the additional sections for extra credit.


#### Additional Resources:

Do you know of a good plain-english explanation of databases? [Email us](mailto:curriculum@theodinproject.com) or [fork](https://help.github.com/articles/fork-a-repo), add it here, then [submit a pull request](https://help.github.com/articles/using-pull-requests).

### Tying it All Together

You've got an idea of what the pieces look like, now it's time to see how they all dance together in a typical Ruby on Rails application.  Read through [The Anatomy of a Web Application](http://www.buildingwebapps.com/transcript/79327-anatomy-of-a-web-application) (you can listen to audio of it by clicking the link on the left side) and pay particular attention to what's happening on the client vs the server side.  It gets a bit more into the guts of what Rails is doing, and this will be a valuable first step towards understanding what you'll be building.  Don't worry if you don't understand what Models, Views, and Controllers are exactly doing, but start to get familiar with that terminology.

### Additional Topics:

#### Git 101

We mentioned git briefly in the previous unit ([Becoming a Web Developer](/becoming_a_web_developer/becoming_a_web_developer.md)) but this time you'll actually start using it.  

If you recall, git is the version control system used by developers.  It means that you can revert to a previous (working) version of the application if you really screwed something up and it means that you have a standardised way of managing a project with contributions from multiple developers.  It's even useful if it's just you and you're working on a project on your own with a few half-baked ideas that you're trying to code at the same time but want to keep separated until they've matured sufficiently.  

It sort of feels like if you were typing a text document and, every time you saved it, you entered a summary message like "just finished paragraph on how git works".  Then, if you realize at the end of the day that all your changes are awful and ruin the flow of the document, you could go back to the last save of yesterday and just bring the document back to the way it was.  The way most people type up a document, they could perhaps just erase the offending paragraphs and move on.  But the changes you make to your web application will be scattered in a dozen different files and will likely involve changing existing code at least as much as it involves actually producing new (and easily deleted) code, so having that ability to just reset the clock to a particular point in the past saves you from having to remember exactly what was changed and what it looked like beforehand.  The power of git goes well beyond this simple example, but it should help you start to see why people use it. 

LEARN GIT:
LEARN GIT:
LEARN GIT:
DO GIT:

#### Testing 101

Like git, testing is one of those things that people often don't think about when they decide to learn about web development but it's critically important to the production of professional quality applications and it will save you tons of time and headache in the end.

Let's say you're building a simple website and you've got a couple of pages linked together with a simple navigation bar at the top.  You make some changes to the code and want to know if the website still works.  So you open up your local version of the webpage and click through each of the buttons on the navigation bar to make sure they each still lead to the right location.  Not too difficult, is it?  It doesn't take too long, and it doesn't seem like such a bad way of doing things.  

But now imagine that you've got a dozen pages with a login system and content that's meant to look different depending on which type of user you are logged in as.  You could come up with a checklist of all the buttons you'd have to manually click on and all the times you'd have to login as a different user but how long do you think it would take to do all those steps before you were satisfied that your changes didn't accidentally blow up some obscure but necessary function of your website?  Situations like that should yell "automate me!" in your head, and that's exactly what testing does.

On the back end, you will learn RSpec, a language that is written in Ruby and one which will help you execute a broad and flexible script of tests to make sure your application is still working the way that it should.  RSpec's syntax even reads sort of like English, though it still takes some getting used to.  RSpec lets you test very specific areas of your application like pulling from and saving to the database or (with some helpful gems) will let you also test the broad-scale interactions the user will have when traveling from one page to another.

On the front end, we'll use a language called Jasmine to do a similar sort of thing.

Everyone does testing a little differently.  Some teams still rely heavily on a QA department with people manually executing checklists like we described in the example above.  Some people use an approach called Test Driven Development (TDD) in which they write the (failing) test first and only then do they actually write the code necessary to make it pass, and thus very deliberately build the application out with 100% test coverage.  Others prefer to keep their test suites fairly light and will only write tests for the major interactions on their pages and any bugs that they have to fix along the way (to make sure they don't come back).  Regardless, testing is highly important and you'll be quite familiar with it by the end of this curriculum.  You'll see tests even before you're actually writing your own... how else do you think we process code submissions?  Many exercises and projects will start with a batch of tests and have you write the code necessary to make them start passing.

LEARN ABOUT RSPEC

#### The Cloud, Hosting, and Software as a Service (SAAS) 101

You've almost certainly heard of the Cloud before and have maybe also heard of SAAS.  The Cloud is really just a way of saying "stored out on the Internet somewhere", which really means "stored on someone else's systems that they let us access using the Internet".  With more and more of the world in posession of 24/7 internet access, that's not necessarily a bad thing.  For software, it has been a great thing.  

READ MORE ABOUT THE CLOUD

Not too long ago, you had to buy a machine, set it up with your program, and plug it into the wall to get it onto the internet.  These days, not only can you host your songs and files and emails in the Cloud, but you can actually run your website from servers hosted by someone else (and maybe in another country too).  Companies (like [Heroku](http://www.heroku.com), which we will use later) make it so that all you have to do is push some code their way and they'll take care of firing up and maintaining the servers necessary to get that application "live" and online.  It means that you as a developer can focus more on building cool applications and less on the nuts and bolts of getting them out there.  This curriculum assumes that you'll be taking advantage of existing cloud hosting, so we won't spend much time teaching you about how to set up your own servers.

READ MORE ABOUT REMOTE HOSTING

Another major advance has been application hosting in the Cloud... the true "web applications".  Where before you had to write a piece of software that would work on a particular type of computer (e.g. Windows machines running Windows Vista) and then get that user to install the software, now many of these applications are run completely using websites.  Think about Google Spreadsheets or Evernote or TurboTax... all of these can be run completely online (though they often have accompanying downloadable applications to help you out).  The ability to create this "Software as a Service (SAAS)" gives you tons of great flexibility as a developer -- it means you no longer have to think about the dozens of different types of operating systems and versions that the users could be using.  You just make sure your application can be viewed properly by people using a few different web browsers.  Even better, when you inevitably want to make large-scale changes or just fix some bugs, you no longer have to convince your users to go through the painful upgrade process.  Just push the changes to your sever, and Presto!, your application is updated and good to go.  If there's a problem with the new Ford car model, they need to issue a recall and have everyone go to a mechanic to fix it.  You just push some code to fix the bug and sleep happy.

READ MORE ABOUT SAAS

#### Security, SSL, and Best Practices 101

SSL stands for "Secure Socket Layer".  This isn't a major standalone topic but it's important to start thinking about how the open and bountiful world of the Internet handles issues of security and secure connections.  Security is something that beginning developers don't spend a lot of time thinking about because they've got a lot on their minds but it will occupy more of your time as you start putting real applications onto the internet.  It's something that you need to be familiar with because sometimes simple but incorrect choices can leave your users' data exposed or your application vulnerable to attack.  Some simple best-practices and best technologies go a long way towards alleviating those issues.

There are a couple of basic areas where security is particularly important -- authenticating users, creating secure connections and securing your databases.  Luckily, the tools we'll be learning have already figured out good solutions to most of these problems.

BASIC SECURITY READING

SSL BASIC READING

SSL AND SECURITY QUESTIONS

#### FTP 101

FTP READING


## How Are Websites Built?
>> BECOMING section instead?

### Macro Level: From Client to Developer and Back

// client team handoff, scrum, cards/stories, gogo, circle back, scrum.... debrief.

### Micro Level: What You Do as the Developer

// tech used, who gets spoken to, where debugs are usually needed, when tests are written, how deployment goes, interactions with other team members.

## Principles of Good Programming

// Separation of concerns, be lazy, KISS, 

## Other "Dumb" Questions Answered

Do you still have any beginner questions left over? [Email us](mailto:curriculum@theodinproject.com) or [fork](https://help.github.com/articles/fork-a-repo), add it here, then [submit a pull request](https://help.github.com/articles/using-pull-requests).

## Finish

Now you've gotten your feet wet and I hope you're getting curious to dig deeper.  You should be fairly comfortable typing commands into your computer's command line and you should understand what happens when you enter a web address into your browser and it returns a functioning page.  You should be able to create a basic web page and make it do some basic things with Javascript.  You should also be able to write a simple Ruby script and describe what Rails and Backbone actually are.

## Additional Resources