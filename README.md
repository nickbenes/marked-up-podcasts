# marked-up-podcasts
Discussion of a new way to markup podcasts for enhanced content.

Revolutionize the Podcast Ecosystem
===================================

Why is this the state of the art in podcast advertising?

Why am I shown ads for post-menopause treatment while listening to a Medal of Honor recipient on *The Art of Manliness*? *Really?*

Come on, people. We can do better than that. Together.

What if instead I had a link to [CPT Bucha's page on wikipedia](http://en.wikipedia.org/wiki/Paul_Bucha)? Or saw a more relevant ad from the sponsor for that show? (In this case another podcast called [The Art of Charm](http://artofcharmpodcast.com).) What if I could donate to the show right there with a single touch, and without leaving the app?

Podcasting is coming into its own, but to keep it growing the revenue model needs to mature. [What if podcasting today is where the web was 20 years ago?](http://www.internethistorypodcast.com/2014/10/the-webs-first-banner-ads/)

Something's Happening Here
--------------------------
We are at the dawn of a revolution in podcasting. [*Serial*](http://serialpodcast.org/) has made that very clear, with over [5 million downloads and streams](http://www.theguardian.com/technology/2014/nov/18/serial-podcast-itunes-apple-downloads-streams). New collaborative networks like Gimlet Media led by Alex Blumberg and Radiotopia led by Roman Mars are leading a growing trend of high production value storytelling podcasts in the spirit of Ira Glass and *This American Life*. More traditional podcasts -- typically some combination of news, interviews, panel discussions, and ports from broadcast radio -- are reaching wider audiences thanks to word of mouth as well as new, improved, and more convenient apps like Stitcher, Overcast, Instacast, and Apple's own Podcasts app.

Advertisers are taking notice. According to a recent [*Slate* article](http://www.slate.com/articles/business/ten_years_in_your_ears/2014/12/podcast_advertising_how_serial_and_other_shows_benefit_from_their_rambling.2.html), CPMs for *Serial* and the Gimlet podcasts *Startup* and *Reply All* can range from $25 to even $100 CPM -- 2x to 6x the cost of a YouTube ad. Pitches from the trusted voice of the host rather than a canned commercial keep the listeners attention, and innovative approaches like Gimlet Media's up-front, documentary-style spots add to that effect. Add to that the difficulty of skipping past the ads (compared to, say, DVR), and it makes sense that more and more sponsors are backing the medium.

Show Me the Money
-----------------
Sponsored audio endorsements during the podcast are only one way to monetize, though. In general, funds come from one of the following:
- **Audio endorsement**: Typically read by the host, these spots are usually similar to traditional commercials. Timing varies, but often there are bookend series of quick endorsements at the beginning and end, along with 2-4 longer spots during the podcast.
- **Donations**: Popular with public radio affiliated podcasts, donation asks take a few different forms:
  - *Crowd funding*. In the past year or two, podcasts such as *99 Percent Invisible* and *Serial* used Kickstarter to fund production for additional seasons. *99 PI* included stretch goals that corresponded to more employees (and thus more shows), better employee benefits, and even the formation of the new Radiotopia network. Even earlier, *Planet Money* funded a [T-shirt series](http://apps.npr.org/tshirt/#/title) that traced production from the cotton farm to the garment factory to the actual shirt that listeners got as a crowd funding perk.
  - *Web payment*. A more traditional model (though still often with donation perks) is to point listeners to a website and do the usual credit card payment there.
  - *Text message*. Also popular is to have listeners text some word to an SMS short code. Messaging and data rates may apply. But you already knew that.
- **Products and Services**. The exact flavor of this varies widely, but some podcasts follow the "freemium app" model and serve (at least in part) as an early step in a marketing funnel for a paid product or service from the podcast producer. In some sense the *Planet Money* T-shirts or other crowd funding perks could be considered examples of this, though most listeners probably think of those as NPR-style donations. More generally, podcasts like [The Art of Charm](http://artofcharmpodcast.com) and [Entrepreneur on Fire](http://www.entrepreneuronfire.com/) bring in some of their revenue via paid courses, books, consulting, and other products and services related to the free podcast content.

Podcast apps can monetize, too. But in almost all cases they do so via banner ads that often have little relevance to the podcast content. Content producers (shows) and content presenters (apps) have almost no synchronization on advertising.

So What's the Problem?
----------------------
The problem with all of these revenue streams is a lack of immediacy. *A lot* of podcast listeners catch up on podcasts in the car, at the gym, doing chores, etc. They're not at their computer ready to enter credit card info. They may remember a website or brand well enough to google it, but they're likely to forget the promo code or `/whatever` to add at the end of it. And good luck remembering to "text 'foobar' to 859236" for the 20 minutes between when you hear the number and when you get out of the car.

It Doesn't Have to Be That Way
------------------------------
Podcast apps could present links, images, and advertisements relevant to the podcast content, and timed to appear at the appropriate point in the show. They could even save a linked article for later reading, fill out a ready-to-send donation text message, or store a listener's credit card information for easy donations and purchases.

None of these are hard to do, either from a technology or from a production standpoint. They haven't been done because they haven't been done. To make them happen it takes a few things:
- Shows with metadata about what enhanced content to display and when. For smaller shows this is unrealistic, but many shows already have a post-production process that includes reviewing the entire show to clean up audio and create show notes or transcripts. For these shows, annotating times to display show-note-level content would add relatively little to the process.
- An app to display enhanced content. This would require some modification to an existing app, but should not be much more complex than including banner ads.
- A common language (a.k.a. *schema*) to communicate metadata for enhanced content. The most obvious way to do this is to extend the RSS specification with several properties in a new namespace, similar to the additional properties required to submit a podcast to iTunes.
- (Very helpful, but not required) A simple tool for adding this new metadata when preparing a podcast for submission to iTunes or Stitcher. In the end, producers will have to communicate what to show and when to show it, but in a perfect world they shouldn't _have_ to learn how to hand-tune RSS XML.

That's what this site is all about. We'll talk about these issues in the wiki, but first one more thing....

Get the Incentives Right
------------------------
A lot of the impetus for this project came from listening to Dubner and Levitt talk on *Freakanomics* about the behavioral economics of a podcast pledge drive. Given that, we would be remiss to _not_ ["Think Like a Freak"]() and talk about players and incentives.
- *Advertisers*. 
  - Incentives here are the usual. 
  - Displaying a hyperlinked visual ad at the same time as the audio endorsement combines the benefits of both.
- *Podcasters*. 
  - Displaying hyperlinked visual ads in conjunction with the audio spot means they don't have to rely on listeners remembering a special promo code or web address, so ads can be more immediately effective and advertisers can more accurately attribute the source of their traffic to the podcast. 
  - Having a button to immediately make a donation will likely make fundraisers far more effective. 
  - Product and service podcasters can link to their sites directly from the podcast.
- *App developers*. 
  - They will be the ones ultimately determining how enhanced content is displayed, so they should be incentivised to make these displays effective. 
  - Displaying podcast-recommended ads rather than guessing at banner ads is likely to have a much better conversion rate, and the app developer should have a share in ad revenue for traffic coming from these ads. 
  - They should also have a share in donation revenue, for example by including a tracking id with the donation and receiving payment equal to some percentage of donation funds attributed to their app. 
  - Displaying other enhanced content (such as relevant but unpaid links or images) is harder to incentivize, but has the potential to make an app more popular with listeners. 
  - Ads for podcaster products and services fall somewhere in the middle. Maybe they pay a CPM, PPC, or PPA rate to the app, or maybe it's just included _gratis_ like other unpaid links or images.
- *Intermediaries and automated tools*.
  - Matching up enhanced content to podcast audio takes work, so this opens up a new market for software developers and service providers to help podcast producers with that work.
  - Attributing ad or donation traffic to a service provider or software product means these groups could share in revenues and be paid in proportion to the value they add rather than charging a flat up-front or recurring fee to the podcast producer. This potentially means a lower barrier to entry for new or smaller podcasts and more meaningful incentives for the people who work behind the scenes to make enhanced content work.
- *Open Source Schema*.
  - We'll work together to develop a metadata schema so all the players can communicate what to show and when.
  - This development has to be open in order to be effective.
  - For now, the plan is to develop the schema on the Github wiki and track issues as usual there.
  - For now, the plan is to make this metadata part of the RSS feed for the podcast. We do this via XML tags with a dedicated namespace. The working namespace is `MUP` for "Marked-Up Podcasts".

Help us make the world of podcasting better for everybody!
==========================================================
For more info, email me at nickbenes@gmail.com.
