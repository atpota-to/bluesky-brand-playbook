# Understanding Bluesky

## Backstory

In 2019, the CEO of Twitter announced an internal research project called "Bluesky". The goal was to explore the feasibility of creating a decentralized protocol that could power Twitter and other social media platforms. After a couple of years and an initial funding pool of $13 million contributed by Twitter, Bluesky became an independent organization with zero ties to Twitter. In late 2022, Bluesky privately launched its new social media app to a small group of test users. The app was very similar to Twitter, but it was powered by what became known as the AT Protocol.

## The AT Protocol

While you might be tempted to gloss over the decentralized technology that underlies Bluesky, learning the basics of it can be extremely helpful in both understanding the Bluesky culture and also tapping into the unique opportunities it can provide.

On a traditional social media site like Twitter or Facebook, all of the user data is controlled by one centralized entity — a for-profit corporation — and stored within that entity’s database in a proprietary data format that will only work with their app. If that social media app goes rogue, declines in quality, or gets bought by a billionaire, then the users don’t have much of a choice in the matter... they either have to forfeit all of the followers and content they amassed over a long period of time or continue using the platform despite all of its toxicity and general crappiness.

The AT Protocol was built to solve this problem. 

You can now own your social networking data, take it with you wherever you want, and never be locked into an app ever again.

### Where your data is stored

When you create an account with the Bluesky app, you’re actually creating an AT Protocol account, even if you don’t realize it. This account uses a standardized and interoperable data model that any developer, company, or person can connect to. When you make a post on Bluesky, reply to another user, or like an image, all of that data gets stored in your account’s Personal Data Server (PDS). The PDS is basically just a file folder containing lots of different files that gets stored on a server in the cloud. You as the user can decide which company (or even yourself) gets to “host” your data. By default, new Bluesky accounts have their PDS data hosted on one of many different Bluesky servers, each of which is named after a different type of mushroom.

`` 
list of mushroom servers
``

If Bluesky were to ever shutdown or become hostile, users could move their data to a new host and still maintain all of their likes, followers, and posts. 

Think of it like your email provider. There are many different companies that provide email hosting services such as Gmail, Outlook, and iCloud. If you ever want to, you’re free to download all of your email archive and contacts and import that data into another email provider instead. The reason this is possible is because all of these companies chose to build their product on top of the decentralized protocol that emailing technology uses.

In that sense, the AT Protocol is sort of like email but for social media.

### How your data is stored

Every single post, like, reply, or follow you make on Bluesky is stored in your PDS in the form of what is called a Lexicon record.

For the non-technical in the audience, a Lexicon is basically just a file format for the AT Protocol... think of it like a file on your computer that might come in many different sizes and shapes: .jpg, .pdf, .doc, .txt

These "file formats" are called NSIDs and look like domain names that are backwards. Here's what Bluesky's "file formats" look like under the hood:

``
app.bsky.actor.profile
app.bsky.feed.like
app.bsky.feed.post
app.bsky.feed.repost
app.bsky.graph.follow
``

Each of these files contains some of your data that is created from an app like Bluesky. By using services like atp.tools, you can see all of the data that lives within a Bluesky account's personal data server. Pretty neat, right? What's even better is that anyone can create their own "file format" for whatever suits their needs, and any app can easily support any other file format at the app developer's discretion.

This is how the new "decentralized" versions of TikTok, Instagram, Goodreads, etc are able to work so easily. You sign into them with your Bluesky (AT Protocol) account, and they support many of Bluesky's native "file formats" out of the box. No need to write a new bio, upload a new avatar, or create a new username for every account... you simply sign in to an app and it all gets imported "magically".

The AT Protocol is still relatively new, but already there are some exciting "file formats" for the AT Protocol that can do interesting things like help you manage events, chat with friends, or write long form blog posts.

There’s a lot more happening under the surface, but that’s all you need to know for now. You can always read more at your own discretion over on the AT Protocol website.

## How Bluesky is different from Twitter 

Now that we’ve gotten through the technical side of things, let’s get to the fun stuff. I said at the beginning of this guide that Bluesky was basically a decentralized version of Twitter, and while that’s true, Bluesky has many features that Twitter (now X) never had. We’ll go through each of these features briefly in this section, but we’ll circle back later on to talk about how to actually leverage these features to be effective.

1. Custom feeds (algorithms)

Perhaps its flagship feature, Bluesky has become famous for how it allows anyone to not only choose which algorithm their feed uses, but also build their own. Gone are the days of being forced to scroll through a non-chronological feed containing posts from random accounts you’ve never followed. For creators and brands, this means that your primary goal is no longer just “appeasing the algorithm”… because there isn’t just one singular algorithm to please.

2. Advanced feed/reply preferences

Hidden under the surface of Bluesky are a plethora of user customizations that anyone can make that apply to the “Following” feed (the reverse-chronological feed of posts from accounts someone follows) and beyond. For instance, users can disable seeing reposts, quote posts, and replies. Within threads, users have the option of ordering the replies however they want: most liked, oldest, newest, prioritize following, hot, or even random (aka “Poster’s Roulette”. 

3. Third-party moderation services

After the AT Protocol launched, there was a lot of talk about the concept of “composable moderation”, which basically just means a suite of tools and infrastructure that would enable any third-party to provide moderation services on top of the network. After awhile, these tools finally started to exist and since then many experiments have popped up as a result. The most well known of which at this point is most likely a service called Blacksky. Blacksky was created by a member of the black community and provides a safe space for Black community building. Users can report posts/content to this third-party service and filter content out of their feeds based on it instead of Bluesky’s official moderation.

There’s even a moderation service that automatically detects and flags screenshots from other prominent social networks like X and allows users to hide that content from their feeds completely. So, cross-posting by using screenshots might not be the wisest idea.

Bluesky also has “moderation lists” that any user can create or subscribe to. On a basic level, they are just lists of accounts, but you can use them to automatically block or mute accounts in bulk with one tap. For instance, there are a series of semi-popular moderation lists for blocking or muting all accounts that follow more than a certain number of accounts (10,000+, 50,000+, etc). Lists like these allow people to keep follower farmers away from them before they even have a chance.

4. Labelers + content filters

Connected to third-party moderation services are a special tool called “labelers”. A labeler… well, it applies labels to things. There are moderation labelers that allow you to hide, warn, or filter posts/accounts based on specific labels (i.e. like the screenshot labeler mentioned earlier), but then there are also vanity labelers that allow users to self-identify with communities, causes, and more by applying a voluntary public label to their own account. For instance, there’s a [vanity labeler for Swifties](https://bsky.app/profile/eras.bsky.sh) that lets them add a little “flair” to their profile in the form of their favorite Taylor Swift Era. Custom labelers of all types and sizes can be created by anyone, though the process to do so is still quite technical at this time.

5. Advanced reply/quote settings

Not only can you turn off replies to your Bluesky posts, but you can also customize reply permissions in extremely granular ways. For instance, you can specify that only users on a custom list can contribute to the conversation or make it so that someone has to be following you in order to reply. Additionally, you can prevent people from quoting your post completely. Both of these features are even available to apply retroactively.

6. Domain names as usernames

Ever been frustrated when joining a new app and learning that your username of choice has already been taken? On Bluesky, this problem is not nearly as significant thanks to the fact that all usernames on the network are actually domain names. When you create a new account, you can get a default username that looks like `name.bsky.social`, but you can (and should) setup your own. 

Using your own domain name is also Bluesky’s native form of self-verification. There are no “blue checkmarks”, but people can verify that your account is legitimate if its username is your domain. For instance NPR (National Public Radio) has the username of @npr.org, which is also its official website. There are even many official government accounts that can be quickly identified by their country’s government domain structure (such as .gov in the United States).

You can even setup subdomains as usernames, so if you are a company or part of an organization you could setup team member accounts such as name.brand.team. Bluesky itself does this for many of its employees—check out the CEO’s handle: @jay.bsky.team

7. Free, open API

Back in the day, Twitter used to have a free and relatively open API. But when Elon Musk took over, he quickly shut that down and started charging exorbitant prices to access its data. If you’re unsure of what an API is or why its significant, just compare the vibrant ecosystem of third-party integrations and applications that exists on Bluesky with what X has today. Bluesky is like a lush beautiful garden filled with lots of diverse plant life, and X is a vacant backlot with some old and dying landscaping. An API is merely a highway that developers and creators can use to retrieve and send data. With Bluesky, that highway is open, free, and let’s you explore the world. With X, only the wealthiest can drive on the highway and there are speed traps everywhere.

An open and free API means an environment friendly to innovation, network effects, and the public good.

8. Everything is public

Speaking of the public, almost everything you do on Bluesky at the moment is publicly accessible data (even blocks and likes). This won’t matter that much to brands, organizations, and creators who explicitly want their content to be public, but it might matter to some of the people in your audience or community. Stay mindful about it, and just know that there are long-term plans to introduce some form of private accounts or content in the future. 

9. In-app media players

On pretty much every other social platform, you and your audience can’t share a link to YouTube or Spotify or some other platform and just have the media play natively. You’d have to navigate outside of the social app and to YouTube in order to play the video. On Bluesky, this isn’t the case. You can listen to music or watch embedded videos without having to leave the app.

11. No outbound link suppression

Since we’re on the subject of sharing links, now’s a great time to mention that another defining and powerful feature of Bluesky is that it doesn’t suppress and down rank content that contains links to outside websites. This is huge for companies, brands, and creators… you no longer need to perform silly algorithmic gymnastics just to convert followers into website visitors.

Also, some people think that Bluesky doesn’t have an algorithm, but this actually isn’t true. Bluesky comes with two feeds out of the box: 1) Discover, and 2) Following. Discover is Bluesky’s proprietary suggestion algorithm similar to TikTok’s “For You” feed. The difference of course is that no one has to use the Discover feed or even have it appear in their app at all… you can disable it completely and rely upon the Following feed, another community-made feed, or a custom feed of your own design.

12. Paragraph breaks in bios

It’s a small detail, but Bluesky profiles have good flexibility in terms of how you can format your account’s bio, Making your description look nice and be readable isn’t a chore that requires tedious tricks or gimmicks.

13. Starter packs

One of the difficult parts of joining a new social network is finding accounts that share your common interests and values. Bluesky tackled this issue head on by introducing an industry-first that was soon copied by Meta/Instagram: Starter Parks. At their core, Starter Packs are just hand-curated lists of accounts that anyone can make combined with an invite-link. By sharing a Starter Pack with someone, they can create a new Bluesky account and follow a bunch of relevant accounts instantly. This feature works especially well for community building, whether that’s for a city (Boston!), a fandom (kpop!), or even bicycle riders. If you’re a brand, you could setup a Starter Pack that has your entire team in it.

14. Nuclear block

Bluesky has intentionally tried to cultivate an environment where users have more control over who can interact with them. One of the ways they achieved this was through what is known as the Nuclear Block. When two people are engaged in a reply conversation on Bluesky, if one of them blocks the other person, then the entire thread of conversation becomes blocked from viewing for everyone else. This feature is a bit controversial, having divided the community into two camps: people who love it and people who hate it. There’s not much that can be done about it, so it’s good to just keep in mind if you ever run into a situation where you see a “blocked” message in a thread.

## The Future

It’s only been a year since Bluesky opened its doors to the public, so we’re still in early days. There are lots of planned features and improvements that the Bluesky team has talked about. Here are a few of the things that we can likely expect in the future:

1. Private data/accounts 
2. Edit button
3. Premium subscription
4. Additional verification options
5. User-friendly PDS management
6. Native analytics

``
Key takeaways:
``
