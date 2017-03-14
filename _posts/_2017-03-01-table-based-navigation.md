---
title: On the current practices in the design of table-based navigation in apps for iPhone
---

# On the design of table-based navigation in apps for iPhone

I'm interested in creating revolutionary new ways that humans and computers can interact: I'm analyzing current practices of software design, to understand what's working, and what isn't.

* * *

In the iPhone app development ecosystem, the influencers are Apple with its 'HIG' (_Human Interface Guidelines_---[link](https://developer.apple.com/ios/human-interface-guidelines/)), A

## Introduction
The problem of navigation fascinates me. First let me explain what I mean by navigation. In using an app (or any technology), the actions the user can take fall into one of two categories, and a simple metaphor will illustrate them: when you drive, your actions support the goal of getting somewhere, but when you fill the tank, that supports the *car*; and it's this second class of actions that includes _navigation_, which in the context of software design refers to moving around within the app (_eg_ in order to expose various functions).

_Navigation_ considers:
<p delete-line/>
- How the app is organized.
- How the user is supposed to move around within the app.
- How easy it is to get to different parts of the app.
- How easy it is to understand what the different parts *are*, that the user can get to.
- How does the user understand *where he is* within the app, what he can do there, and where he can go next from there.

One way to organize an app is like a table; and this is the kind of navigation we're going to talk about.

### The table view
The _table view_ is one of the standard user-interface components that Apple provides, and most apps that are navigated like a table employ this component, so it will form the foundation for our discussion. Before we consider it at length, let me show you what a table view looks like in a simple form:

<img src="/assets/2017-03-01-table-based-navigation--table-view-1.svg">

### How humans look at things
Everything we look at we construct in the mind, and an essential inquiry lays the foundation: What is this thing I'm looking at?, and what can I do with it? If you look at a hammer, you identify it as the tool by that name that fits with your understanding of it, and you know from experience that you can drive nails with it, for example. We say a hammer _affords_ its user the capability of driving nails, and in interaction design we call anything the user can do with the interface an _affordance_.

When we regard a user interface, such as on an iPhone screen, we seek to understand what it is we are looking at, and what we can do there.

When we regard something, we harbour a question in our mind, What is this thing I'm looking at?---And what can I do with it?

How do we know it's a table view?---I ask this from the point of view of the user---this seems to me to be an important first question. We recognize it as a table view by visual cues:
<p delete-line/>
- A slightly darker region at the top appears divided from the lighter-coloured region below it.
- If there are two regions on-screen appearing deliberately divided, we are led customarily to suppose the larger region to contain 'content,' and the smaller one, something *about* the content, and this suggestion is especially pronounced if the smaller area be of a different shade.
- Apple categorizes regions on the iPhone screen as either bars or views, and the darker region at the top is called a _navigation bar_, which is a standard component that, though it can be dressed up, maintains certain qualities so as not to lose the 'look' that makes it recognizable as a navigation bar.
- To be precise, the navigation bar is not considered to be part of the table view, however it does help us recognize the table view, which occupies the remainder of the screen.
- The regular horizontal lines suggest 'rows.'
- That these row-dividing lines don't extend completely to the left of the screen, it creates a vertical continuity that strengthens that the rows together form a kind of region that is separate from the navigation bar.
- The chevrons that point in the natural reading direction are naturally and customarily interpreted as suggesting there's 'more,' and the simplicity of the touch screen input medium offers only one natural and customary gesture to access this 'more:' the (single) tap.
- If we move our eye from the leading edge (_ie_ the left edge for us English readers) forwards (_ie_ rightwards), we encounter first a vertically-connected margin, then a region demarcated by row-dividing lines, where each row also contains some content (in this case the labels, _One_, _Two_, _Three_), then finally that chevron suggestive of further content; and so we have a gradation in three steps from higher to lower levels of abstraction, and this subtle order is comforting for our subconscious.

Let's consider this slightly more involved table view:

<img src="/assets/2017-03-01-table-based-navigation--table-view-2.svg">

We've added two elements, a title and a 'back' chevron. This 

<!-- ## Introduction

### What this is about
I'm interested in creating revolutionary new ways that humans and computers can interact. My journey begins by considering the designs that are currently being produced by the software industry; and trying to understand what's working, and what isn't.

This analysis is about taking something apart so we know how it works. The thing I chose to take apart is the iPhone app I use most: it is Overcast, a podcast app by Marco Arment. (Overcast is one of the best-designed apps out there, and the care and thoughtfulness Mr. Arment has poured into it have produced a quality beyond what Apple is capable of. I'm not kidding.)

### About the app
<aside in-the-margin><figure><img class="small" src="/assets/2017-03-02-overcast-design-analysis--overcast-logo.svg"></figure></aside>

- _Overcast_<sup>&reg;</sup> by Marco Arment.
- Link to app website: [overcast.fm](http://overcast.fm).

To describe what Overcast is, in simplest terms: it is an app that affords the following fundamental capabilities. The user can:
<p delete-line/>
- manage a list of podcasts (from the list of all available podcasts)
- for each podcast, manage a list of episodes (from the list of all avaiable episodes for that podcast)
- play a podcast

### The scope of our analysis
Right now I happen to care about the design of the navigation: *not* how the app fulfills the user's goals, but how the user is able to move around within the app. (This is the most fundamental aspect of any app.)

## Deconstructing Overcast's navigation

### The root navigation screen

<img special src="/assets/2017-03-01-overcast-design-analysis--root-navigation-screen-0.svg">
In order to reason with agility, we will simplify the screens into symbolic representations. To begin, consider the figure above; this is how the app looks in its root navigation screen. Next, let's constrain our attention to include the screen only:
<img special src="/assets/2017-03-01-overcast-design-analysis--root-navigation-screen-1.svg">

Let's simplify to the essentials, and we'll consider the resulting wireframe:
<img special src="/assets/2017-03-01-overcast-design-analysis--root-navigation-screen-2.svg">
The essential elements of the root navigation screen are the status bar (1), the navigation bar (2), and the table view (3). The status bar (1) is that thin band at the topmost region of the screen, displaying information such as the current time. Moving our eye downward, the navigation bar (2) is next, and to be exact, its region of the screen actually starts from the very top of the screen, so that it goes *under* the status bar. The table view (3) is the region distinguished by a blue (rather than gray) boundary; that is where in our example the podcasts are listed; and the table view's function *generally* is to list a screenful of items from a larger list, to provides a viewport---as much as one screen can show---into a larger list of items. And to denote that the region contains more than one screen can display, I have chosen to use a dashed line to indicate that more elements exist 'below' the lower boundary.

### The table view

Let's consider what this navigational element is like, the table view.
<img special src="/assets/2017-03-01-overcast-design-analysis--root-navigation-screen-3.svg"> -->


<!-- ### About the app
<aside in-the-margin><figure><img class="small" src="/assets/2017-03-02-overcast-design-analysis--overcast-logo.svg"></figure></aside>

- _Overcast_<sup>&reg;</sup> by Marco Arment.
- Link to app website: [overcast.fm](http://overcast.fm).

### Preamble
There is a great big technological party, but not everyone is invited. I'm thinking of older people, whose experience in using new technologies is rather frustrating than fulfilling. And it's not their fault: the field of software design is in its infancy: we still don't know how to create except only the most crude kinds of interactions between human and computer. It's an exciting time for someone who has a vision.

This analysis is about taking something apart so I know how it works. The thing I chose to take apart is the app I use most: it is Overcast, a podcast app by Marco Arment. Not only do I consider Overcast to be one of the best-designed apps out there, but I love its creator also, Marco Arment, who has been an outspoken influencer and benefactor to the industry.

* * *

## Why navigation

_Ie_ why is it only the design of the *navigation* that concerns me? --- Keep this question in mind.

### What is _excise_?

Former Apple designer Bret Victor can introduce us to interaction designer Alan Cooper's concept of _excise_:
<p delete-line/>
> Alan Cooper defines _excise_ [...] as a cognitive or physical penalty for using a tool—effort demanded by the tool that is not directly in pursuit of a goal. For example, filling a gas tank is done to support the car, not the goal of arriving at a destination. Cooper goes on to assert that software navigation is nothing but excise:
<p delete-line/>
> > ...the most important thing to realize about navigation is that, in almost all cases, it represents pure excise, or something close to it. Except in games where the goal is to navigate successfully through a maze of obstacles, navigation through software does not meet user goals, needs, or desires. Unnecessary or difficult navigation thus becomes a major frustration to users. In fact, it is the author’s [_ie_ Mr. Cooper's] opinion that poorly designed navigation presents the *number-one problem* in the design of any software application or system...

I believe Mr. Cooper to be right, and if we considered user aggravation in aggregate, it's the design of how apps are supposed to be navigated that forms the greatest contribution to that unhappy culmination. My attention, then, is directed at this special class of excise. (I am also attracted that app navigation is one of those simple problems we should've already come up with a few good solutions for. The decades have given us many solutions, and still we wait for a few good ones. It always fascinates me when the simplest problems go unsolved.)

* * *

## How to list things

In creating Overcast, Mr. Arment had to figure out first how to show a list of things on a touchscreen (those 'things' being either podcasts or podcast episodes, depending on whether the user is looking at the list of podcasts, or having navigated inside a podcast, is looking at a list of podcast episodes). Nor are those things listed supposed to be passive, but interactive in some way, so that tapping on them would do something (_eg_ tapping a podcast navigates inside it).

I want to understand how to list things on a mobile device touchscreen in simplest terms. The screen can show things, and affords that the user can touch and draw what are called _gestures_ on it; so the medium of communication is visual and... indicative (I wanted to say gestural but that would be less accurate)---the user *indicates* things on the screen in expectation that the app is 'paying attention,' and he uses an index finger or thumb for a stylus.

There are three things we do with a list:
<p delete-line/>
- View it (_ie_ its items).
- Change it (delete or add an item).
- 'Invoke' one of its items.

The mobile device touchscreen, being small, provides only a window into the true list, and cannot show all the items simultaneously. The user's eye, having finished reading the on-screen items, has nowhere to go, unless some indicative gesture---that being the only gesture available to 'talk balk' (as we have already implied)---is needed to supplement the visual sense's consuming. The speed of the visual sense does not convene with latency or delay, so it is important that whatsoever this supplemental gesture be, that it be as quick and easy to execute as possible.

If we think about how we used to scroll touchscreens before we had even electricity, it would inform us of which gesture this should be; and though you will think the answer to be obvious, maybe you never thought to get there in this way. Before electricity, we had a touchscreen, but you'll have to humour me. The touchscreen, so to speak, was in operation whenever we would *draw*. Imagine the very mechanics of putting pen to paper to draw. You place the point on the page, and I will suggest you have started a data feed. You are about to scroll through a list of positions your pentip 'is' in relation to where you want it to be: in other words, there's the curve that you want to draw, and the actual curve your hand draws; and these two curves would diverge significantly if not for the fact that as you form your line you are constantly advancing your view of them while correcting any minute discrepancies between them. So here we have a form of scrolling already popular even before touchscreens. And we are reminded how intimate the hand is with the eye, how practiced they are in coordination. So it feels natural that the dragging gesture



Developers have relied on Apple's guidelines for direction, as well as thinking of the generally-accepted user-interface idioms, which last is like a tradition of how user interfaces are understood to work.





For lists of things on an Apple mobile device, there a



 The accepted user-interface idiom concerning navigating a list is via scrolling it (with a finger).




<figure><img with-border src="/assets/2017-03-01-overcast-design-analysis--root-navigation-screen-0.svg"></figure>

<figure><img with-border src="/assets/2017-03-01-overcast-design-analysis--root-navigation-screen-1.svg"></figure>

<figure><img with-border src="/assets/2017-03-01-overcast-design-analysis--root-navigation-screen-2.svg"></figure> -->