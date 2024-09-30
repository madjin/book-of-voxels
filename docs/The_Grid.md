---
title: The Grid
description: Part 1 navigates projects, infrastructure, and prototypes involved in designing an internet city as a fully digital 3D world.
image: https://xrdevlog.com/img/grid.jpg
robots: index, follow
lang: en
dir: ltr
breaks: true
disqus: xrdevlog
---

# The Grid

{%hackmd theme-dark %}

Part 1 navigates projects, infrastructure, and prototypes involved in designing a digital city owned by its users.

Originally published June 2019

###### tags: `devlog` `grid` `cv` `janus` `desert`

> “The Grid. A digital frontier. I tried to picture clusters of information as they moved through the computer. What did they look like? Ships, motorcycles? Were the circuits like freeways? I kept dreaming of a world I thought I'd never see. And then, one day I got in...” - Kevin Flynn

This dev log is a collection of ideas revolving around the concept of 'the grid' or a virtual city. Some of the goals with this is to not reinvent the wheel, focus on compatibility over invention, and start simple to allow for emergence.

![](https://i.imgur.com/suSGVNN.jpg)

> **If the internet were a city, what would it look like?**

![](https://i.imgur.com/qIuuq99.jpg)

Projects that we can potentially integrate:

- [Dat protocol](https://dat.foundation)
- [Exokit](https://exokit.org)
- [Janus / Vesta](https://madjin.github.io/janus-guide/#/)
- [Hubs / Spoke](https://hubs.mozilla.com)
- [MSF](https://github.com/smsithlord/MetaShortcutFormat) - Rich presence for shortcuts in 3D worlds as seen in [Anarchy Arcade](https://www.anarchyarcade.com)
- [Opensea](https://opensea.io) - Digital collectibles marketplace
- [Decentraland](https://decentraland.org) 
- [Cryptovoxels](https://www.cryptovoxels.com) - Virtual world built on Ethereum blockchain

One of the ways we can integrate XR projects (starting with WebXR) into this vision is to establish camps for different themed content. Think of this as a spatialized new tab page. Through curation we establish an oasis within the vast ocean of content that exists on the web.

![webxr.today](https://i.imgur.com/mVFjbkY.jpg)

Another reason for building this hub for content is for directing the flow of traffic between virtual events and gatherings of all sorts. For example, what are the areas that people hang out in before / after going to the VR cinema or concert? 

Many VR platforms already have portals and menus between worlds within their own ecosystem, perhaps this concept can be expanded on to glue content between the platforms more seamlessly. Maybe this is the missing ingredient for making cyberspace feel more like a place rather than a dream we are all chasing.

See world traversal event notes <https://github.com/m3-org/world-traversal>

---

### How's it work?

In order: 0. Physical -> 1. Startpage -> 2. Home Space -> 3. Street

![](https://i.imgur.com/44jcBZL.jpg)

- Can choose to stay offline or go online
    - If offline, can still communicate with local nodes via mesh
    - If online, user can walk from their home space to street or teleport

0. Physical Layer

Just ask, don't want to give away everything.


1. [**Startpage**](https://github.com/madjin/startpage)

The browser is the killer app. Even as there are many devices per user, many feel right at home when they're able to connect to the web. This feeling is especially true in the context of personal web pages and social media profiles - the current internet of self.

![](https://i.imgur.com/FVrZitL.jpg)

See example: <https://i.imgur.com/FVZRmpB.mp4>

The startpage example I have is meant to serve the simple purpose of shortcutting to your favorite content. The design is inspired by windows/linux/osx desktop environments.

![](https://i.imgur.com/qkPbNnh.jpg)

Bai has created a 3D window manager using elation engine in this example. The windows are composited with z buffer. Demo: <http://vrcade.io/hack>

2. [Home Space](https://github.com/madjin/home-space)

Working on the shell to be something modular such as a shipping container.
![](https://i.imgur.com/4VHO5tq.jpg)

The inside as seen from Anarchy Arcade
![](https://i.imgur.com/Iz4GfKs.jpg)

Websurfaces to productivity software and entertainment in the JanusWeb version.
![](https://i.imgur.com/aOP1NyI.jpg)

Work-in-progress Hubs version of the Home Space. There will be a .glb file and spoke scene.
![](https://i.imgur.com/yNiPz7l.jpg)



3. Street

The street / grid is the connective tissue of the 3D web, akin to the 

![](https://i.imgur.com/Ojr3FTK.jpg)

![](https://i.imgur.com/iN9hduF.jpg)

[Vesta](https://vesta.janusvr.com/) is the town square for WebXR content. Implements a JS spatializer for trending content.
![](https://i.imgur.com/ftzeYgJ.jpg)

Cryptovoxels is a dynamic world to discover content, with links spread throughout the city.
![](https://i.imgur.com/kW5UvQZ.jpg)


---

![](https://i.redd.it/zrddcwv7axj21.jpg =100%x)

---

### Space

We could use a generalized data visualization system to map and traverse web content or discovery nearby nodes. 

![](https://i.imgur.com/D98s2Eb.gif =100%x)


This system can be useful throughout the process to mind map, debug, and navigate potential opportunity zones that may otherwise get overlooked.
![](https://i.imgur.com/F4X1yQ2.jpg)



---

## Desert Town

The desert base layer
![](https://i.imgur.com/ayWm7zu.jpg)
Demo: <https://vesta.janusvr.com/bepis/desert>

![](https://i.imgur.com/TRznQCz.jpg)

[Spyduck](https://spyduck) has created a procedural parcel generator for Janus with an in-world editor that detects when objects go out of bounds. However, such a system is a form of reinvention for what [Bnolan](https://twitter.com/bnolan) has already accomplished. It's a big ask for people to own another home in a new city.

Demo: <https://tachibana.cyberium.club/the_city/dev/dim_1?x=0&y=1&z=0&dir=NW>


#### Land

It's better to stand on the shoulders of giants, especially with the web. Cryptovoxels has minted approximately 1200/3026 parcels in Origin City as of 6/22/19. Origin City (Cryptovoxels) is about 4% the size of Genesis City (Decentraland) and ~0.2% the total marketcap. These projects are taking different approaches to build virtual worlds on the Ethereum blockchain that one can get further detail of in another post.
![](https://i.imgur.com/M12ZfEr.jpg)

We have strong representation in the [Makers District](https://github.com/madjin/makers-district) of Origin City that we can use as a base The entire community is super collaborative in general and we hold great connections to whales with hundreds of parcels combined. This can make it easier for us to deploy city-scale experiments such as the advertising model [Spyduck has made](https://www.cryptovoxels.com/play?coords=N@215E,8N).

#### Origin City Desert

![](https://i.imgur.com/ul0NPAY.jpg)

![](https://i.imgur.com/m7vhC21.jpg)

![](https://i.imgur.com/2fKQcR7.jpg)

#### Origin City Dark

![](https://i.imgur.com/GW3kTa5.jpg)

This picture shows ourselves are walking in Origin City from Janus like ghosts from another dimension. We're headed east to Makers district to build things.

![](https://i.imgur.com/xZMXFlx.jpg)




#### Art

There's always amazing crypto-art on display in Origin City with many interesting galleries [worth visiting](https://www.cryptovoxels.com/play?coords=S@447E,115N).

Creation/Curation Tools:

- <https://supermedium.com/supercraft/>
- <https://aframe.io/a-painter/>
- <https://hubs.mozilla.com/spoke>
- <http://anarchyarcade.com/>
- <https://github.com/jbaicoianu/janusweb>
- <http://www.xrartisttoolkit.com>

Cryptoart platforms and marketplaces:

- [Opensea](https://opensea.io)
- [Opensea storefront](https://twitter.com/opensea/status/1141800576113680385)
- [Superrare](https://superrare.co)
- [Firstedition](https://firstedition.art)


#### Ad blimps 

Pay BTC/Stripe to advertise: <https://tachibana.cyberium.club/mockingbird/start>
![Blimps](https://i.imgur.com/jn9Tpkg.jpg)

The same ads for the blimps can get mirrored across the virtual world as well. We could tag the entire city with markers that will display an uploaded image someone paid for.
![](https://i.imgur.com/Kkh9hwM.jpg)
Tag parcels with this banner: <https://tachibana.cyberium.club/mockingbird/get_ad/image/1x1/0>

#### Tickets
[Opensea](https://opensea.io) willing to help with coding <https://docs.opensea.io/docs/developer-tutorials>
![Tickets](https://i.imgur.com/JGNh2yp.jpg)

You can buy NFT tickets from the 3D world using Ethereum, USDC, and DAI as long as you're signed in [metamask](https://metamask.io) from your browser. The operator can use the Opensea API with the machine to get a percentage from sales and secondary sales.

Tickets do not have to be used for 1 platform, they are generally a means of having an appointment with some event in the real or virtual world. An interesting use for tickets is in the realm of education. I'm curious if platforms like [Bigscreen](https://bigscreenvr.com) would allow for 3rd party ticket services to be used for users to book events, professional meetings, or trainings.

#### Vending Machines 
View dev log: <https://xrdevlog.com/cryptomachines.html>
![](https://i.imgur.com/NW7aQhl.jpg)
Demo: <https://vesta.janusvr.com/bepis/lut-dcl>

#### Teleporters
shortcuts to virtual worlds plastered like stickers on the box
![](https://i.imgur.com/yBId5kS.jpg)


**Media**

- <https://i.imgur.com/k2GW07W.png>
- <https://i.imgur.com/CvhJKOc.jpg> - DCL map
- <https://i.imgur.com/Idtkug1.jpg> - Lut Gholein, perhaps our finest quality work in JanusWeb

---

### The Street

Neal Stephenson has said that the Vegas Strip inspired him when writing about 'The Street' in Snow Crash. Knowing that Decentraland and Cryptovoxels have made grids, I'm curious if a single long street can thread a large chunk of the metaverse somehow.

> Stephenson's Metaverse appears to its users as an urban environment, developed along a single hundred-meter-wide road, the Street, that runs the entire 65536 km (216 km) circumference of a featureless, black, perfectly spherical planet. [Snow Crash Wikipedia](https://en.wikipedia.org/wiki/Snow_Crash)

![](https://i.imgur.com/QkkhzbX.jpg)

- <https://streamable.com/kymun> - The Strip experience
- <https://xrdevlog.com/vegas.html>
- <https://github.com/janusvr-examples/vegas-strip> - JanusWeb demo source



---

### Metacade District

The Metacade district, an industrial hacker arts district with arcades and nightclubs. This could serve as a smaller more botique neighborhood experience. The roads / parcels can also be procedural generated if we wanted to expand beyond 8-9 current parcels.

![](https://i.imgur.com/vuYliMz.jpg)

![](https://i.imgur.com/CsP8VXu.jpg)

Read more about Metacade here: <https://xrdevlog.com/metacade.html>


---

## Inspiration

These examples are inspiration while thinking about 'The Grid'.

### Kowloon walled City 
Because the grid does not have to be flat.
![](https://i.imgur.com/Cwn5RdN.jpg)
Large cross-section: <https://www.thisiscolossal.com/wp-content/uploads/2014/11/full-size.jpg>

Notes:

- <https://twitter.com/ExUtumno/status/1141354217774428160> - Wave Function Collapse
- <https://github.com/mxgmn/WaveFunctionCollapse>
- <https://www.youtube.com/watch?v=-W7zt8181Zo> - Demo with links in description


Real world adaptions:

- COD Black Ops
- <https://twitter.com/hkdevblog?lang=en> - HK Game
- <https://www.youtube.com/watch?v=V_2KgQOqzBc> - Japanese arcade

---

### The Stacks

Continuing on the trend of vertical as well as horizontal, 'The Stacks' inspired a generation in the best seller novel Ready Player One.

![](https://i.imgur.com/cpodXkb.jpg =100%x)

One can imagine that each trailer represents a [home space](https://github.com/madjin/home-space).

---

### Burning Man

A temporary city emerges in the desert once each year. It is a gathering of art, music, and culture that attracts people from all walks of life to camp in the desert for seven days/nights.

- No currency
- Focused on self, creativity, and collaboration.
- No trace left behind when it's over.

Burning Man organically grew out of an annual tradition and is still heavily resisting any type of commercialization. The concept is all about disconnecting from the modern world into an alternate reality.

Burning Man organizers say that attendees need to bring all of their supplies because only two items are sold on-site: coffee and ice.

In 2015, Burning Man took in $36.9 million in revenue, nearly all of it from ticket sales, while the non-profit spent $35.8 million to host the event, according to tax documents.

Tickets cost $450 and $100 for parking this year, with 68 percent of attendees said they spent between $1,000 and $5,000 in total on tickets, supplies, travel and other costs last year. <https://burningman.org/culture/history/brc-history/census-data/>

<https://burningman.org/timeline/2016>

Comparing Event Prices:

Bonnaroo (4 days): Between $274.50 and $349.50 + $59.75 vehicle pass + fees
Coachella (4 days): $399 + $99 camping pass + fees
Electric Daisy Carnival (3 days): Prices range from $249 to $599, vary by location
Glastonbury (5 days): ~$300 + $50 car parking + fees
Burning Man (8 days): $390 + $80 vehicle pass + fees

Media:

- Timelapse 2011 <https://www.youtube.com/watch?v=ZQacfYW6eZQ>
- Hyperlapse 2017 <https://www.youtube.com/watch?v=-8dOCu2WJcM>
- Decentraland Walkthrough <https://www.youtube.com/watch?v=OEXRRaYjuwM>
- Valerian scene <https://www.youtube.com/watch?v=FXjXUOeczVM>




---

### Earth

Earth is the original grid with its own established geolocation coordinate system, borders, and preset content. By using planet Earth as the VR base reality we can very easily adapt our creations further into the AR spectrum with later iterations.

Bai has been working on interplanetary scale Earth 2.0 experiments since atleast 2012, a time when the elation engine was built for epic space flight and combat.

<https://www.youtube.com/watch?v=cbHi7zbAwao> webgl earth flyby (elation engine 2012)

These companies allow developers to build applications with location data: 

- <https://scape.io>
- <https://www.6d.ai>
- <https://ubiquity6.com>
- <https://www.mapbox.com>
- <https://www.openstreetmap.org>

**Notes**

From the World's Best Selling Game comes Minecraft Earth

- <https://www.minecraft.net/en-us/earth>
- <https://www.theverge.com/2019/5/17/18627341/minecraft-earth-ios-android-free-ar-game-features-pokemon-go>

Done some experiments to augment real-world places such as DNA Lounge in SF where we had a party in a 1:1 3D recreation of the venue to celebrate the 20th anniversary of The Matrix.

![](https://i.imgur.com/TQJQAdP.gif =100%x)

- <https://www.youtube.com/watch?v=BCSz3Ltob34> - GITS cyberpunk city

It'd be interesting to accumulate a collection of 3D scanned physical spaces, reimagine them with XR magic, and then experience them like a video game. Earth animation studio can be useful to help make cut scenes.

---

### Writer Thoughts

The best way to explain some of these concepts is through creating a proof of concept demo, which is about 60% completed right now. 

[JanusVR](https://madjin.github.io/janus-guide/#/) devs are exceedingly good at rapid prototyping ideas which can then go on to become more mature products. Another startup in this area includes [Torch](https://www.torch.app) which has been IOS only but is now working on an [android version](https://www.torch.app/android) soon too. We're big fans of collaboration.


> ### Interconnected Spaces
> Suppose that in the Metaverse your company owns an office, in a building, in a city. It is easy to imagine how this might happen . The city might be a popular destination for commerce, with appealing tax rates for the type of work your company does, and the building you work in might be a popular destination for companies offering the same kind of services you do. Furthermore, the appeal of having the office, building and city all be spaces that are connected together  —  meaning you can look out the window of the building and see other buildings  —  is due to the fact that our memories operate best when things are organized  as physical structures that don’t change much over time. So we will want a way to connect spaces that are hosted, served or operated by many different people and companies into a stable, larger space, and this mechanism must be one that can be easily edited by those content creators and operators.

> With the web, the connective tissue is the hyperlink, where one site links to another one through the "doorway" of clicking on a block of text or media. For the Metaverse, the strategy seems likely to be one in which developers can create volumes of space or literal doorways that link to other servers. So, the owner of the "building" server can link the space contained within one of the offices to your "office" server and visa-versa. In this way, larger spaces can be created (the city, for example) comprised of many different nested layers of servers, with the boundaries between these servers not needing to be visible at all. - [Parts List For the Metaverse](https://www.highfidelity.com/blog/parts-list-for-the-metaverse) by Philip Rosedale


Bnolan has been thinking in this space for awhile:

- <https://medium.com/@bnolan/the-grid-a-digital-frontier-7269fb934711>
- <https://medium.com/@bnolan/fontus-501efd5a9b>
- <https://medium.com/@bnolan/generating-a-live-map-view-of-cryptovoxels-b8d1e68a067>

Couple other great reads that have inspired this writing:

- <http://singularityhub.com/2015/08/26/a-makers-guide-to-the-metaverse/>
- <https://loupventures.com/the-metaverse-explained-part-3-economics/>
- <https://github.com/RangerMauve/local-first-cyberspace>


## To be continued

Part 2 will contain content and demos that aim to clarify the ideas discussed here.