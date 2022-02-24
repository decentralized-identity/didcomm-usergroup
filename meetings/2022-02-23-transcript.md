Daniel Hardman — Yesterday at 12:03 PM

Welcome to the UnSync meeting, everyone! We will be in meeting mode for approximately the next 12 hours. I will post the agenda below. Please say "hi" on this thread, then read through and comment on the agenda items, using this thread as the place to chat during the meeting.

Reminder: if you have not already done so, please schedule this recurring meeting in your calendar for every other Wednesday, at a time convenient to you.

Agenda: https://github.com/decentralized-identity/didcomm-usergroup/blob/main/meetings/2022-02-23.md

Re. agenda item 1, say hi: Hi from Daniel Hardman (SICPA).

Re. agenda Item 2, charter: here is Proposal A -- we ratify the charter as currently written (follow link in agenda). Please leave your votes as thumbs up/thumbs down on this message.
(vote: 7 thumbs 0, 0 thumbs down)

Re. agenda item 3, repos: anybody want to advocate a different repo approach?

Daniel Hardman — Yesterday at 12:29 PM

Re. agenda item 3, repos: Who wants to volunteer to be a maintainer, given the maintenance duties/procedures linked in the agenda?

Re. agenda item 4, the book: here is Proposal B -- This UG agrees to formally take on the task of writing a DIDComm Guidebook, and that we do so by taking over and improving the content of the current "Implementers Guide" that was started by the DIDComm WG. Please leave your votes as thumbs up/thumbs down on this message.
(vote: 5 thumbs up, 0 thumbs down)

Re. Proposal B: I have opened a PR to do what I'm proposing. However, this PR is separate from the general proposal. So you can go look at the PR to get an idea what content we might be writing, but don't vote for or against the proposal based on the PR. The PR is a separate topic and I suggest that, if proposal B passes, we spend a couple weeks discussing, with the possibility of voting on the PR at our next UnSync.

The PR is here, BTW: https://github.com/decentralized-identity/didcomm.org/pull/26

Re. item 4, the book, here are some brainstormed topics from me:

1. When and how to use DID rotation.
2. How to do distributed timeouts.
3. How to debug connectivity issues.
4. Hello World for DIDComm (using one of the implementation libraries; pick your preferred lang from among 5 supported)

Re. agenda item 5, feedback: I'm not sure whether putting the meeting in a thread is best, or whether we should stay in the main channel. Curious to get your reactions.

Also, I am wondering how we summarize meetings permanently (since threads archive after a while). Maybe we ask @dbluhm (who will close this meeting at the end of his Wed workday) to copy the transcript to a .md file in /meetings/ folder in our group repo?

Also, I am wondering if we should just switch from Discord to Github conversations. It would possibly entail less work for the chairs (since the data and the conversation would both live in the same place), but it de-emphasizes Discord, which DIF is trying to get everyone to.

TelegramSam — Yesterday at 3:46 PM

Hi! Sam Curren Here.

Nice PR for the book @Daniel Hardman! That's a great start.

On Thread vs Main vs Github conversations: I don't think it matters for the purpose of meetings. DIF is experimenting with Discord as a slack replacement, but I don't think having meetings elsewhere is any problem. We should use the best tools for the job.

Book Brainstorming Ideas:

- What is DIDComm and why would I use it? (super high level)
- Why developing a protocol on top of DIDComm is a great idea.
- Protocol Design Basics
- Protocol Design Best Practices

Daniel Hardman — Yesterday at 4:01 PM

@TelegramSam : thanks for weighing in. Do you have a vote on either of the formal proposals?
  Snorre Lothar von Gohren Edwin — Yesterday at 5:11 PM
  I just want to say hi, Snorre Lothar von Gohren Edwin from Diwala here. I love the initative, but have some hectict days around me right now which means I cannot adda whole lot of input at this moment. Will be back stronger next time!
  Daniel Hardman — Yesterday at 5:18 PM
  Thanks for checking in, @Snorre Lothar von Gohren Edwin !
  Steve McCown — Yesterday at 7:50 PM
  Hi everyone.  This is Steve McCown from Anonyome Labs.  I like the new meeting format -- especially having it as a sub-thread of the main group (can't ever get lost 🙂

I like the charter and am voting to ratify 👍

Regarding example code in the repo, I presume that this will contain group-generated / approved code.  Would it also be helpful to have an 'Example - Links' section where we can point to external didcomm implementation code (OSS apps that use didcomm) that may have originated externally?

Brian Richter (Aviary Tech) — Yesterday at 7:57 PM

1. Hello - Hi all, Brian Richter here. I created one of the implementations (in typescript) which needs a little bit more love once i get a chance. The goal for it is to be able to use didcomm within a modern browser environment.
2. Re Charter - looks good to me (voted w/ thumb up)
3. Re Repos -  I think we should have somewhere to store didcomm related content we come across, with consent of course (ie slides from presentations, articles, social media posts)
4. Re Book - I've thought for awhile now the spec is already a bit of a book.. It's a tough pill to swallow pointing someone to the spec and trying to get them interested. I wonder if we should think about how some of the spec content might make sense to be in the implementers guide. I worry about adoption when the spec isn't an easy pill to swallow but i think I might be overthinking it... just brainstorming. pretty late in the game to be suggesting this..
- As a more solid book topic proposals I would say we should have sections talking about the following (even if they are mentioned in the spec)
    - good and bad DID methods for didcomm
    - Encryption curves / algs (what to use and when)

drummondreed — Yesterday at 8:01 PM

Drummond Reed from Avast checking in here. I already voted on the proposals, which I like very much. RE using GitHub Discussions, I haven't used it much yet but from the description (https://docs.github.com/en/discussions) it does look quite attractive. I'm also liking Discord too, so as long as there is an easy way to archive our "meeting notes" from these meetings, I'm also fine staying here.


There is one downside to making a whole meeting a single thread, however, which is that you can't have subthreads to comment on what someone else said earlier in the meeting. In UnSync meetings, that seems particularly useful. So a thought is just to use the main Discord channel for the meeting, then copy the whole chat from start to finish out for archiving. If it happens to include some non-meeting topics, that's fine too, it will be easy to recognize those.

BTW, I personally won't have much time to contribute to the Book (outside of maybe some sections about DIDs), but I expect I might be able to get other resources at Avast to contribute. Just give me some time to see who else I can interest.

Brian Richter (Aviary Tech) — Yesterday at 8:14 PM

testing a reply to the thread message

drummondreed — Yesterday at 8:14 PM

Brian! It works!! I didn't think you could have a thread inside a thread! Slack doesn't allow that. Okay, now I'm even more impressed with Discord.

Ignore my comment above 😄

Brian Richter (Aviary Tech) — Yesterday at 8:16 PM

just wait until we have a didcomm alternative to discord

drummondreed — Yesterday at 8:17 PM

I can't wait!!!!!!!

Daniel Hardman — Yesterday at 8:43 PM

I started a "rich chat" protocol based on DIDComm. Several others did, too. However, I had to pause mine when I asked how to include more than 2 people. I realized I had to solve the n-wise problem first. So I think I did that (https://github.com/decentralized-identity/didcomm.org/pull/13), and now I want to collaborate with people on the DIDComm chat protocol. That could be a UG topic...

drummondreed — Yesterday at 8:44 PM

Isn't that what @Steve McCown and his team is working on now?

Daniel Hardman — Yesterday at 8:44 PM

I dunno. Steve, please enlighten us!

drummondreed — Yesterday at 8:45 PM

BTW, I like the term "rich chat". We could also call it "agent-assisted chat" or "smart chat".

Daniel Hardman — Yesterday at 8:51 PM

All these technologies are in the same basic category: Signal, Discord, Rocket.Chat, Slack, Teams, WhatsApp, Telegram, WeChat, FB Instant Messenger, etc, etc.

Every one of them locks you in to a vendor (https://daniel-hardman.medium.com/security-silos-and-sovereignty-522e30bb8eb4) -- you can use the great features, but you can't carry your relationship anywhere else.

Email clients are the same way.

What I want to do is reinvent this stuff so the relationships and conversations belong to the people who have them, not to the platform that enables them. I want to continue on email a conversation I started on signal. I want all the features of the best of these chat tools, plus I want offline, plus I want to be able to run arbitrary co-protocols (schedule a meeting, run an UnSync, pay for lunch, run a vote, take a test) right inside the conversation by invoking a DIDComm co-protocol. I want DIDComm-style attachments, too (where I can attach by bittorrent reference, not just by value). Etc.

Medium: Security, Silos, and Sovereignty
Why portable security is the sleeper — but killer — feature for SSI

drummondreed — Yesterday at 8:56 PM

+1000. I love that vision.

swcurran — Yesterday at 11:08 PM

Stephen Curran here -- Cloud Compass Computing Inc./BC Gov.

Read through, voted. I quite like this approach to meetings.

Regards the book -- I think a big thing we'll need is how to migrate from DIDComm v1 to DIDComm v2.  If we can't get that done there will be a split.  Not sure if that is a separate book vs. a part of The Book, but it's something that I think we need to get to as soon as V2 is ready -- or perhaps before.  This might be something that is already available and I've missed it.

Brian Richter (Aviary Tech) — Yesterday at 11:13 PM

great point stephen. I think a migration guide should be front and center of The Book. Theres a lot of didcomm v1 out there that will hopefully eventually be on v2.. that migration sounds messy to me I hope we can find a clean solution

Daniel Hardman — Yesterday at 11:15 PM

I agree that this will be good. I think it's possible to write a python script that can convert a v1 msg to a v2 msg (and back), but that might not do 100% of the work.

I've had such a script on my to-do list for a long time. Haven't had a lot of time in past 6 months, but my work responsibilities are shifting to where I can justify DIDComm a bit more (even if I can't justify other identity stuff so much). So maybe...

Writing such a tool (or attempting to) would be good fodder for the chapter -- and vice versa.

JamesEbert — Today at 12:08 AM

1. Hey folks! James Ebert from Indicio. I realize it's very close to the end of the UnSync meeting, but I wanted to chime in even though I've had some unexpected things come up today!
2. Re Charter - LGTM (voted 👍 )
3. I am open to assisting with maintaining 🙂

I can voice interest from me in the creation of a rich chat protocol--even if it's only peer to peer (vs n-wise). I also am interested in understanding and outlining the migration path between v1 & v2. +1 to DID-Rotation.

Rodolfo Miranda — Today at 12:12 AM

Hi, Rodolfo Miranda here. We are a new team called RootsId. We joined forces to build an open source wallet for the Cardano community. As we go, we  are getting involved deeper and deeper. We’ve worked hard in researching and testing several didcomm v2 frameworks that you’ve built (thanks!).
I think we can collaborate with some helloworld examples meanwhile we become more familiar in this WG. I also like the idea of protocols above didcomm; we are also building a didcomm v2 mediator to test our wallet.
Migration path shouldn't be the two protocols running in parallel with a top layer deciding which to use on agreement with the other side?

Daniel Hardman — Today at 12:22 AM

Hi, @JamesEbert. Thanks for coming, and thanks for volunteering to be a maintainer. I have sent you an invitation to be a maintainer on didcomm.org, and I will see about doing the same for the UG repo. Any other volunteers that I missed?

Hi, @Rodolfo Miranda . Excited to get to know you and learn more about your team. Thanks for coming.

Re. migration path: yes, that's the migration path for a running agent. But before the running agent can support both protocols, it has to have code that can produce and consume messages in both formats. Writing the v2 equiv of v1 protocols by hand can be done, but is tedious. That's what the tool mentioned by @swcurran might simplify.

Rodolfo Miranda — Today at 12:31 AM

Got it. Probably can contribute on that as well.

Brian Richter (Aviary Tech) — Today at 7:25 AM

I would like to volunteer to maintain didcomm.org repo as well @Daniel Hardman

Daniel Hardman — Today at 9:24 AM

@Brian Richter (Aviary Tech) : Thank you! I sent a maintainer invitation to you (if I correctly remembered your github handle as @brianorwhatever?)

Daniel Hardman — Today at 9:35 AM

Meeting is closed now (but of course our main channel is always open to keep talking). Summary:

Looks like 8 or 9 of us noted our attendance. I think that's a nice first effort. Thanks to everyone who came.

Proposal A (ratify charter) passes 7-0.

Proposal B (take on the task of DIDComm Guidebook) passes 5-0.
We got some volunteers to act as maintainers (thank you, James and Brian!). If others want to volunteer in the future, let us know.

We got some excellent ideas for the Guidebook; Daniel B or I will compile them. Let's keep that as an open brainstorm topic, too. Next meeting, we'll be asking if anybody wants to start working on a section. No pressure, but an invitation...

The idea of making DIDComm v1->v2 migration easier got onto our radar.

See you again in 2 weeks.
