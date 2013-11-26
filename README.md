DYCONV
======
A vision of a free-form group chat system that sees to a number of the glaring flaws in the status quo, IRC.

PROBLEMS SOLVED
---------------
* Able to reply to interesting parts of the backlogs and revive conversations that never deserved to die. [without causing undue distraction from whatever the group has moved onto since.]
* Prevents off-topic or otherwise uninteresting conversations from dominating the channel and killing leagues of innocent conversations yet to be conceived.
* Allows off-topic or otherwise subjectively uninteresting conversations to take place anyway, and provides methods for other people in the channel to notice them and join right in if that's what they're into.
* It's possible to have one on one conversations without going through the awkwardness or suffering the constraint of it being fully private, nor do you have to clog up any channel with very . users.notify(new conversation(topics/channel). It will be a new bubble discoverable according to its topics/channel/participants.

[Things we might as well fix while we're at it]
* You don't need to host a fucking bouncer to have access to the backlog[though public logging for channels can be optional, of course]
* user icons and more detailed public profiles. Yes, this is necessary. IRC is a place where networking occurs, and 10 character names are not sufficient characterization for most people to remember the interactions and observations they have had with a person.
user icons may be simple geometric shapes[no dick pics up in your face, provides a consistent look, can assign a generated icon to users who couldn't be bothered configuring their own.]
* detailed user profiles are of course optional, as is a real name.
it might be a good idea to generate little audio chimes for people as well.. why havn't I explroed this area.
* knowing whether your friends are around[if that's information they grant you].


PROBLEMS INTRODUCED
-------------------
?

MOCK UPS
--------

x

VISION DETAIL
=============

When a user views a channel, they see a number of **conversations** with with varying levels of detail proportionate to their **salience ratings**, in separate partitions of the screen. One may fill half the screen, another may only show a few lines at a time, some might just be minimized to the point of being pixels that flash every time a comment gets posted indicating only than that there are more conversations going on.
Dyconv tries to have a memory. It supports centralized logging*. Though active conversations may be represented almost entirely as the linear sequences we're familiar with on IRC already, if you're doing any amount of backlog reading, the conversations would be better represented and explored in a tree structure. Many subconversations were started as replies to some comment older than the most recent. For a moment they would be seen embedded, indented in the main conversation[the matter of which thread is the 'main' thread[displayed in line with what it is a reply to rather than indented] is subjective, it is whichever subthread you're focussed on, or has the most salience for you.].
Anyway, as a result of this, there should be two interaction modes which can be switched between easily, **reading** and **engaging**.

A dyconv channel has many conversations. A **conversation** iss a frontier of activity. The **salience** of each conversation iss a function of any of the following list of conversation aspects, in any combination, dynamically adjustable during usage.

In decreasing order of importance(

, The amount of activity in the conversation.

, the people involved[and how much you care about each of them]

, whether the conversation is a direct offshoot of a conversation you were involved in, and how involved you were at the point of the reply[if you wrote the comment it's replying to, you WILL be notified.]

, the keywords it contains. Or perhaps just #topic tags, which we can expect to be invoked when a user wants to draw the attention of people who might be interested in the conversation.

, whether the conversation is a direct offshoot of a conversation you were approximately involved in.

, Explicit registrations of interest in given conversations or their ancestors.

, Channel-specific user-voted metrics. Channels could do all sorts of creative things with this. One example might be HootingVolume, how many of the participants are /hooting. Hooting would be for when things are getting  _really_ _dramatic_. Like, big disruption to status quo.

, Other.

)
