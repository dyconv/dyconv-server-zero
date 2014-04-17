![logo](http://i.imgur.com/IVjZL3x.png)

DYCONV
======
A concept for a better free-form group chat system. A general solution to a large number of underobserved flaws in the status quo, IRC and Twitter.

To cut to the chase,

PROBLEMS SOLVED
---------------
+ Able to reply directly to interesting parts of the backlogs and revive conversations that never deserved to die.
+ Prevents off-topic or otherwise uninteresting conversations from dominating the channel and killing leagues of innocent conversations yet to be conceived.
+ Allows off-topic or otherwise subjectively uninteresting conversations to take place anyway, and provides methods for other people in the channel to notice them and join right in if that's what they're into.
+ It's possible to have one on one conversations without clogging the channel with impenatrably personal dialog, *and* without the awkwardness or constraint of it being fully private.

[Things we might as well fix while we're at it]

+ Standard way of reviewing publicly logged conversation.
+ It's made easier to characterize and remember the people you're interacting with. There are two ways we could attack this. One is making it easy to review past interactions with a person, that lets you build up a profile on them organically and is basically equivalent to a log search. The other way to attack it is with user icons and more detailed public profiles. User icons could be simple geometric shapes, if you like[no wangs, provides a consistent look, can assign a generated icon to users who couldn't be bothered configuring their own.]. Detailed user profiles are of course optional.


PROBLEMS INTRODUCED
-------------------
?

MOCK UPS
--------
tbg

VISION DETAIL
=============

A dyconv channel has many **conversations**. A conversation iss a frontier of activity. Their **salience**, a determiner of which conversations a user is exposed to and how prominent they are in their feed, is a function of any of the following aspects, in any combination, dynamically adjustable during usage.

+ How active the conversation is.

+ Whether you have registered interest in the people involved in it.

+ whether the conversation is a direct offshoot of a conversation you were involved in, and whether you were involved at the point of the reply[if you wrote the comment it's replying to, you *will* be notified.]

+ the keywords it contains. Or perhaps just #topic tags, which we can expect to be invoked when a user wants to draw the attention of people who might be interested in the conversation.

+ whether the conversation is a direct offshoot of a conversation you were approximately involved in.

+ Explicit registrations of interest in given conversations or their ancestors.

+ Channel-specific user-voted metrics. Channels could do all sorts of creative things with this. One example might be HootingVolume, how many of the participants are /hooting.

+ Other.

In the default state, a user's attention is split between multiple conversations. Conversations on the edge of their attention will drop in and out of view as other low-salience conversations jostle for the position. Whenever a user replies to an older comment, a branch occurs. Branched conversations will be visible indented within the main line, but once the fronteirs of activity reach a certain distance[say, once it's been scrolled off-screen by the activity on the main frontier], a branched conversation may be considered separate. To remain in view it will have to vie for the salience to afford its own window alongside the rest of the conversations in the channel.

This allows many distinct threads to organically emerge and coexist.