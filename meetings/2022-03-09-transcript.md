## Welcome

Daniel Hardman — Yesterday at 12:26 PM
Welcome to the UnSync meeting, everyone! We will be in meeting mode for approximately the next 12 hours. I will post the agenda below. Please say "hi" on this thread, then read through and comment on the agenda items, using this thread as the place to chat during the meeting.

Reminder: if you have not already done so, please schedule this recurring meeting in your calendar for every other Wednesday, at a time convenient to you.

Agenda: https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-03-09.md

## Chat

(I am running the meeting in the main channel this time, not in a thread, to see if we like it better.)

Snorre Lothar von Gohren Edwin — Yesterday at 1:13 PM

Hi all!  Have a good meeting!
3. Getting the word out
   I think the newsletter is powerful, and if we can get that into the different groups it would be great. Making a collaborative list of contact poitns and groups with interoperability would also be helpful.
   I will add this to the agenda of next meeting in interop.

No more comments on this
No more comments on the other points
I have one item that was not added. So will do a question right here

10. How kosher is it to do non encrypted messages?
    Split my messages up in threadable sequences

Daniel Hardman — Yesterday at 1:35 PM

@Snorre Lothar von Gohren Edwin Re. #10: My intuition is that the answer to "how kosher" depends on two subquestions:

1. Are you uninterested in confidentiality because the message is intended to be public anyway (e.g., it's a message inviting anyone in the general public to send you a message)?

2. Will the message stay within trust domain boundaries? (That is, Alice sends an encrypted message to Bob; Bob decrypts and wants to send it as plaintext to 5 of his agents, but all of them are within his own sphere of control, and Bob trusts himself.)

If the answer to either of these questions is "Yes", then I think it's totally fine.

If the answer to both of these questions is "No", then I think messages should be encrypted, because it means confidentiality should matter. It might be tempting to say, "True. But I'm using https, which gives confidentiality anyway." This is a fallacy, because by design a sender in DIDComm doesn't actually know the full route to the target. A sender might be using HTTPS, but perhaps part of the route is not. Using channel-oriented encryption (e.g., TLS) on the part of the channel you can see is not actually secure, if someone somewhere has to take plaintext off that channel and put it somewhere else that you don't know about. The guarantee is supposed to be end-to-end. (In my question #2 above, "Bob" is the end; what he does after it gets to him is his business, not DIDComm's. That's why I'm comfortable with him using plaintext in a context wholly under his own control.)

Daniel Hardman — Yesterday at 1:36 PM

^^ This would be a great topic for the Guidebook, ne c'est pas?

@Snorre Lothar von Gohren Edwin : it looks like a part of your comment might have been lost; how does "Split my messages" above relate to the line above it?

Snorre Lothar von Gohren Edwin
started a thread:
Encryption or not  FAQ for the guidebook

Snorre Lothar von Gohren Edwin — Yesterday at 2:57 PM

Sorry, I meant, I split my messages up, so they are threadable segments. F.ex that there can be a #3 thread based on my first comment if someone wants to. Just to keep the context of certain aspects enclosed into itself 😄

Like I did with your quitebook comment/question.

If that would not be a message on itself, that thread could be cluttered with other types of information

Snorre Lothar von Gohren Edwin — Yesterday at 4:23 PM

Re #5 - https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-03-09.md#5-preliminary-pr-on-guidebook: I approved and since the info is already vetted and produced i see no issues. Easier to work with after first framework is in place

Re #6. Volunteers for Guidebook Sections - https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-03-09.md#6-volunteers-for-guidebook-sections

I can try to volunteer to get that part about my question in to the guidebook after the first PR is merged and I can see the context a bit more.

Rodolfo Miranda — Yesterday at 9:30 PM

Hi, Rodolfo Miranda here.

Re 3.1. I'm attending ToIP Tech task force, and some keri WG.

Re 3.3. Podcasters and twitter spaces are mainstream to spread voice. There are a lot of blockchain communities involved on SSI can help too. I'm particularly involved in the Cardano community with many tech discussions and projects going on

Re 4. 👍

Re 5. 👍

Re 6. I can start with some hello world's

John Jordan (BC Gov) — Yesterday at 10:25 PM

Hi all… following along the meeting.

We could definitely schedule blog post with trust over IP… We are working on our editorial calendar and this would certainly fit into Technology stack discussions as well as ways to satisfy design principles

Lance Byrd — Yesterday at 11:14 PM

Hi all.  Lance Byrd from RootsID here for the DIDComm unsync 🙂  My path has been:
    Cardano->
    Cardano Atala Prism (decentralized identity platform)->
    Cardano Catalyst Decentralized Identity Challenge (Cardano community funding for decentralized identity)->
    RootsID/RootsWallet identity software (first DIDComm awareness from @Rodolfo Miranda )->
    ToIP Tech stack->
    DIF DIDComm

I will spread the word from now on about these!  I was in the DIF all hands today with Identity Woman.  I was in DIF DIDComm WACI yesterday (it was only Juan and I).  Several other DIF wgs.  I also attend several ToIP meetings and KERI meetings.  I also run a discord for RootsID.

approved.

i am happy to contribute with @Rodolfo Miranda on the hello world (we already work together at RootsID).

7 (aka 9).  This was super helpful to get plugged in!  I don't know what it will yield long-term but i'm really excited to participate in this way and want to adopt the technique in my own project 🙂

Brian Richter (Aviary Tech) — Yesterday at 11:18 PM

Hi all happy wednesday

I did not receive maintainer status on the didcomm-usergroup repo just didcomm.org

I was not on the mailing list yet and looks like there are only 23 members at this point.. might not be the best place to centralize announcements yet but could be a good avenue down the road

thanks!

approved

I will volunteer to start on the "Protocols" section of the book

Yes

## Summary

Daniel Hardman — Today at 8:28 AM

Hey all, this is Daniel H doing a wrap-up and meeting summary. (Next time it's @dbluhm 's turn.)

Thanks for attending, contributing, reviewing the PR (and to Brian for contributing one!), and volunteering. I am noting the following action items:

* @Snorre Lothar von Gohren Edwin volunteers to write up his Q and my A as a PR for the book, once it's clear where it should go.

* @Snorre Lothar von Gohren Edwin volunteered to add our UG meeting announcement to the agenda of the next DIF Interop WG.

* @Rodolfo Miranda and @Lance Byrd volunteered to work on the Hello World section of the book.

* @Rodolfo Miranda volunteers to spread the word in the Cardano community. @Lance Byrd volunteers to do the same and maybe also WACI, other DIF WGs, KERI, and RootsID.

* @John Jordan (BC Gov) volunteers to schedule a slot for a blog post at TOIP.

* @Brian Richter (Aviary Tech) volunteers to start working on the Protocols section of the book.

I have an action item to figure out why @Brian Richter (Aviary Tech) didn't get an invitation on the didcomm-usergroup repo. I'm on it.

@Brian Richter (Aviary Tech) : can I ask you for a quick favor? Since you do have maintainer rights on didcomm.org, can you please merge the PR that we voted to accept?

I will be raising a PR or two of my own as well between now and our next meeting. (One will be a PR against the DIDComm WG spec repo, removing the guide content which will now be redundant, and updating links in the spec to use our new permalink to the guidebook on didcomm.org.) And I will publish the transcript of this meeting at https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-03-09-transcript.md

@Rodolfo Miranda and @Lance Byrd : re Hello World, you might have a look at the IIW presentation that was given by DSR in Oct 2021. I'll track it down for you. They walked people through sending and receiving a message. You could possibly link to their recording as an extra resource, and/or use the same workflow. One nice thing about it is that the libraries they used have the same interface in 3 or 4 different programming languages, so the Hello World writeup could be almost identical no matter which language a programmer likes.