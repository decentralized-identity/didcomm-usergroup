# DIDComm UG Unsync Meeting - 2022-03-23

## Welcome

Daniel Hardman — Yesterday at 7:41 AM

Agenda published here: https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-03-23.md

## Chat

Daniel Hardman — Yesterday at 7:41 AM

My comments:

Re. 1: hi, it's me. 🙂

Re. 3: I want all new protocols to be searchable at didcomm.org, because the vision is to make that website like the DIDComm equivalent of npmjs.org, pypi.org, or Maven Central. However, that doesn't mean we have to take protocol specs out of Hyperledger Aries. Here is an example of making a protocol searchable on didcomm.org, but keeping the spec in Hyperledger Aries: https://didcomm.org/basicmessage/1.0/. I say we do that, anywhere that Aries is the natural locus of development.
Basic Message
DIDComm lets people and software use DIDs to communicate securely and privately over many channels: the web, email, mobile push notifications, QR codes, Bluetooth, message queues, sneakernet, and more.
Daniel Hardman — Yesterday at 7:46 AM
Re. 9: I am liking this format. But I'm interested to try it once on Github Discussions instead of Discord. I'm curious to know if anyone would be up for that?

Snorre Lothar von Gohren Edwin — Yesterday at 7:50 AM

1: Hi its me again, Snorre! All good in the hood. Getting married soon so my capacity is streched as work and getting things into shape demands most of the time. So just setting extra things on hold until 2nd of April
2-https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-03-23.md#2-follow-up-on-action-items: I have a reminder to do both fo my things, this popping up every day, so I know, but again, the comment on 1 defines the amount of load I can do right now
6-https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-03-23.md#6-preso-to-ccg: I would love to provide input if it happens after my wedding date

Lance Byrd — Yesterday at 10:46 AM

1. Hi Friends, Lance (RootsID) here.

2. I've started working on the Hello World action item:

issue created here https://github.com/decentralized-identity/didcomm.org/issues/31
fork work so far after going through the presentation referenced  https://github.com/2byrds/didcomm.org/blob/book-hello-world/site/content/book/v2/libstools.md
I should have more time this week to add the other sections.
I'll be touching base with @Rodolfo Miranda today.
I attended several of the meetings that I listed but didn't promote our user group at a single one!  i just need to get it top of mind and announce it at the start.

4. Timeouts

Happy to review.  The timing information looks good so far.

9. Last item of business: feedback

I'm happy to have this user group to connect with for my own identity wallet development.  And I like the unsync format.  I'm open to trying Github discussions (i commented in the thread).

TelegramSam — Yesterday at 11:49 AM

1. Hey! Actually setting a calendar appointment worked wonders for getting me here. 🙂
3. Agree with Daniel that hosting or linking as much as possible is the right answer. I lean a little more 'didcomm.org' centric on publishing protocols, particularly new ones. If they are intended for a specific community, leave it there. If they are intended for broad adoption, I lean more heavily toward native 'didcomm.org' hosted protocols.
5. Gatsby - I managed to make a very small change, but mostly got lucky. Part of a Gatsby-ite might be a guide for the rest of us to understand how to make common changes. I'd Love some help here.
9. Left (by way of experiment) in the Item 9 Thread above.

TelegramSam — Yesterday at 11:58 AM

On Book URL: Thanks for making this happen @Daniel Hardman! Is this a stable URL we can use moving forward?

Brian Richter (Aviary Tech) — Yesterday at 2:00 PM

1. Hi hi
2. I didn't manage to get started on protocols section yet but now that the book is on the website I will take a first pass. All good if we can't get me as a maintainer of didcomm-usergroup the didcomm.org repo is more important which I have now
3. I lean didcomm.org for most protocols and if this is the case would like to start pushing this. I am aware of my bias as I am not heavily involved in the hyperledger aries community so take this with a grain of salt. It would be nice to have a central location for all these decentralized protocols 😁 . There was a couple of issues opened in the spec repo for new versions of protocols so this question is an important one to answer..
4. spec PR looks good
5. I tried and failed to figure out how to wildcard route (see https://github.com/decentralized-identity/didcomm.org/issues/20) so no i am not an expert sadly.. I use svelte now and will never go back to something else. 
6. I saw your e-mail and I think a presentation to CCG would be great.. but I really think it would be more appropriate to do it once the spec is stable and "published".. as I know that will be the first thing that comes up. do we have a timeline for that yet? It would be great to say we have a final version ready before IIW
9. I think this is effective and agree with above that doing this in discord shows our activity nicely.. and also agree a threading approach would be great.

swcurran — Yesterday at 6:11 PM

1. Hey y'all.
3.

I'm not a fan of Daniel's suggestion because (a) there is no organization to that site and it will grow unruly, and (b) standalone protocols without community endorsement and an "AIP" concept of a standard grouping of protocols are pretty useless.

Aries RFCs is poorly documented for newcomers.  But it is organized, and those with tribal knowledge know exactly how to use it and share it with others.  Obvs we need to move that from tribal to clear docs. I think if we start fresh with a new place -- especially one that is just a list, we'll have to evolve it all over again before we get something useful.

My vote would be to continue with Aries RFCs and AIP -- adding in the new versions and an AIP v3.0Draft.  Ideally, with some work done in the repo to make it welcoming to newcomers (starting with AIPs vs. stumbling up on it), and archiving a number of dead end protocols (e.g. Rich Schema ones, others that aren't relevant).

My alternative would be YAR (yet another repo) that is managed more or less the same way but that people unwilling to use Aries can live with.

TelegramSam — Yesterday at 8:09 PM

I'm not a fan of Daniel's suggestion because (a) there is no organization to that site and it will grow unruly, and (b) standalone protocols without community endorsement and an "AIP" concept of a standard grouping of protocols are pretty useless.

I'm a fan of improving didcomm.org rather than avoiding it. Let's add the organization we need. Let's figure out how to have something like an AIP where appropriate.  Experience indicates that folks are reluctant to cross org boundaries, even if for dumb reasons.

Daniel Hardman — Today at 5:56 AM

@swcurran : I don't understand why you perceive my suggestion to be at odds with Aries. I'm saying: develop an RFC in Aries -- but index it in addition on didcomm.org, so that site becomes a comprehensive index.

We need to correct the misperception that DIDComm is only a Hyperledger thing. We can't do that if the only place people can learn about protocols is in Aries. It's fine if a protocol is "homed" in Aries, IMO -- but it can't be indexed only there, or else we don't actually have something free from Aries.

Daniel Hardman — Today at 6:06 AM

Regarding "there is no organization to that site and it will grow unruly" -- the site is intended to serve protocols at URLs in the form "https://didcomm.org/protocol/ver". This is an organizational pattern that was chosen by the Aries community, and it has long since been enshrined in every protocol we write; adopting that URL namespace pattern was part of the AIP work you've championed. The website does a great job of making all these protocols searchable. I don't understand what risk you are worried about; are you thinking we need to change it in some way? 
Regarding "standalone protocols without community endorsement and an AIP concept are pretty useless": nobody says that a protocol published at didcomm.org needs to be standalone. As you yourself advocated, an AIP can reference any protocol definition. So publishing the protocol is a first step, but referencing it and drumming up community support is a second step. They are not alternatives to one another.

swcurran — Today at 10:24 AM

Fair enough.  I was thinking about the index generator we have in the Aries RFC repo. While nominally useful, it gave us a false sense of security that we were helping people navigate the site and get value from it.  Even the "status" settings in the generated index were of little value.

If the use of the didcomm.org site is for a developer to look up the ID of a message they received and are trying to understand, what is described is useful. If they are going to the didcomm.org site to "see the big picture", it won't help -- and that's my concern.  It could work, with a lot more effort than is suggested.

Agree that a new place outside of Aries could be a good idea.  My concern is defining and refining specs in the place proposed without context around those new protocols is recreating the "bad old days" of the Aries RFCs repo.

### Thread: Item 9

Daniel Hardman — Yesterday at 7:46 AM

Re. 9: I am liking this format. But I'm interested to try it once on Github Discussions instead of Discord. I'm curious to know if anyone would be up for that?

Snorre Lothar von Gohren Edwin — Yesterday at 8:00 AM

9-https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-03-23.md#9-last-item-of-business-feedback: I dont mind trying out discussions, my only concern is threads on threads, but dont know if discussions support that in a way or not. But seeing htat more and more discussions tools are popping up, such as: https://slite.com/. Not sying we going to use it, but maybe its a good inspo for what is needed to get things going

Suggestion, maybe we can thread each item some easy way? Like I tried here? The first person posting a reply to an item, that someone wants to reply to, can thread it? Including item 1, which I did not do now just to show a difference. But then each item has to be seperate messages for that to work 

Snorre Lothar von Gohren Edwin

 changed the channel name: 
Item 9
 — Yesterday at 8:01 AM

Lance Byrd — Yesterday at 10:35 AM

The nice part about using Discord is when people come to the user group they see our activity.  Showing vibrant signs of life is important for momentum (either in Discord or Github).  We have to decide if new participants are more likely to land/connect in Discord or Github discussions.  There might be some other benefits from Github discussions that i'm not accounting for... similar to all the integrations with issues/branches/PRs.  I'd like to hear what others who have used Github discussions have experienced.

TelegramSam — Yesterday at 11:43 AM

@Snorre Lothar von Gohren Edwin I was thinking about a similar adjustment: What if the Agenda was posted item by item? The Item itself becomes the start of the thread to discuss it. Keeps things organized, and we can see all the related discussion for each point grouped together.
Having said that, I'm totally open to other ideas and platforms. Trying several and seeing the common success in between them will guide us to what the requirements for a platform ought to be
@Daniel Hardman Discussions are not enabled on the didcomm-usergroup repo. Do you see an option to turn it on for some experiments?

Snorre Lothar von Gohren Edwin — Yesterday at 1:47 PM

Why I made my suggestion so "complicated" was because it was to avoide Daniel having to make threads and the github document. So we would crowdsource the thread based on when people chimed in.

I agree on that keeping discord environment active is a concern, but we dont have the answer to where people arrive. So maybe try to choose some metrics for what we want to achieve here and see if it is met or not?

## Summary

dbluhm — Today at 10:58 AM

Wrap-up and meeting summary 🙂 

Action items picked from the comments:
- @Snorre Lothar von Gohren Edwin to follow up on action items from last meeting when time permits after wedding (Congratulations!)
- @Lance Byrd to continue work on Hello World section of book and to touch base with @Rodolfo Miranda 
- @Lance Byrd to provide review of timeout PR when ready
- @Brian Richter (Aviary Tech) to start working on protocol sections of the book

Some open questions:
- From @TelegramSam: "Is [the book URL] a stable URL we can use moving forward?"
- From @Brian Richter (Aviary Tech): "Do we have a timeline for [when the spec will be stable and 'published]?" Would be great to have before IIW
- Discussion on Item 3, where next gen protocol specs live, continues 🙂
- Still seeking someone experienced with Gatsby.

Summary of Feedback (Item 9): The general feeling I'm getting is that people are open to experimenting. Several opinions were expressed in favor of continued use of Discord and particular interest in agenda items having their own threads to keep relevant messages together.

Thanks for your participation! I'll get the transcript and summary pushed to the UG repo shortly.
