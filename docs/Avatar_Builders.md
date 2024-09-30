---
title: Avatar Builders
description: Exploring programs use to create 3D avatars with as we work on building open source alternatives.
image: https://i.imgur.com/p97HJ0f.jpg
robots: index, follow
lang: en
dir: ltr
breaks: true
disqus: xrdevlog
---

# Avatar Builders

###### tags: `devlog` `m3`

{%hackmd @themes/dracula %}

[toc]

---

- https://github.com/M3-org/avatar-interop/wiki/Avatars
- https://hackmd.io/@XR/avatarlod
- https://hackmd.io/@xr/wearables1
- https://github.com/m3-org/ready-player-m3

![](https://i.imgur.com/EFLnf25.png)


Avatars are the audio-visual representation of self and the spiritual successor to social media profiles. This dev log explores the ways we create our avatars from what's popular / trending to the open source solutions folks in M3 are building.

---

## Open Source

M3 folks have been discussing and building open source projects to create your own interoperable metaverse avatar with.

![](https://i.imgur.com/yNfSZBx.jpg)

Working in public allows us to more easily collaborate with other working groups whom are developing or fostering discussions for open standards.

- https://omigroup.org/
- https://metaverse-standards.org/
    - [Kent Bye interview](https://voicesofvr.com/1098-metaverse-standards-forum-unites-leading-standards-orgs-xr-companies-towards-open-metaverse-interoperability/)

### Blender

- https://github.com/saturday06/VRM_Addon_for_Blender

Swiss army tool for 3D. Used to create, kitbash, optimize, and convert all sorts of files. Can be used headlessly, like in the case of [Ready Player Me](https://www.blendernation.com/2021/03/08/behind-the-scenes-ready-player-me-3d-avatar-creator/).

{%youtube 7qV5UKChCys %}
Watch on Youtube: https://www.youtube.com/watch?v=7qV5UKChCys

### Avatar Creator

- https://github.com/AtlasFoundation/AvatarCreator

Closest thing we have to open source Ready Player Me style character creation. Basic functionality and UI is there, try your best to ignore the placeholder 3D assets.

:construction: This software is still in pre-alpha :construction: 

![](https://i.imgur.com/97bDPrd.png)

Export functionality for VRM / GLB / Screenshots is already implemented (although still has some bugs to fix)

![](https://i.imgur.com/GclrIWn.png)

The assets are loaded in via json. We can implement some kind of schema here for each item, such as additional metadata for describing future objects that are created by someone / come from a certain collection.

The models are currently attached to VRM armatures which is why it's .vrm, but they can be glb also.

See: https://github.com/donmccurdy/glTF-Transform

Can add metadata to glTF files themselves also.

![](https://i.imgur.com/JhE6rYP.png)

Devs really like the idea of a plugin to export 3D models + json for loading into Avatar Creator straight from blender. Can have different categories for different attachment points. M3taloot is mostly setup for this.

### M3taloot

- site: https://m3taloot.com
- thread: https://twitter.com/dankvr/status/1507189063694131202

![](https://i.imgur.com/2Vjv2fd.png)

![](https://i.imgur.com/EW1vbHr.png)

![](https://i.imgur.com/Eyml7S5.png)

![](https://i.imgur.com/uXmtEPX.gif)

![](https://i.imgur.com/7axFvuH.gif)

sign-in with wallet, see synthetic loot + keyblade?

---

### Boomboxhead Tools

Boomboxhead is working on a Unity tool to export 3D files + json that target different metaverse platforms. It can also be used to render animations and video.

![](https://i.imgur.com/YLFqr2L.jpg)


![](https://i.imgur.com/363zrL3.png)

![](https://i.imgur.com/ztPL1Oo.jpg)

Exporting to glTF

![](https://i.imgur.com/N7Ym6Sc.png)
![](https://i.imgur.com/yoH8W7c.png)


Export VRM with UniVRM?

Combine ingredients from:
- Metarick
- M3
- Boomboxhead


![](https://i.imgur.com/LbytuJP.gif)


![](https://gyazo.com/4d934a2c6b494ba603d5147fcedb88f5.gif)

Avatar randomizer but it can export all, including the scene, and create worlds. JSON can export to multiple targets like glTF, json, webaverse, anarchy arcade, etc.

![](https://i.imgur.com/4HJw2xY.png)

baked out in hierarchy?
can asset be shot out by a bullet?
can you tip your hat? is baked to mesh?




**Dev log 1**
Watch on Youtube: https://www.youtube.com/watch?v=squiTzamUrk
{%youtube squiTzamUrk %}

**Dev log 2**
Watch on Youtube: https://www.youtube.com/watch?v=TpJiyPq4OM4
{%youtube TpJiyPq4OM4 %}

![](https://i.imgur.com/qDycPH1.gif)


![](https://i.imgur.com/NeKrOAh.png)
![](https://i.imgur.com/OkHLulV.png)
![](https://i.imgur.com/WTMe0sg.png)

![](https://i.imgur.com/5AsqTud.png)

![](https://i.imgur.com/twFYiWS.gif)

| ![](https://i.imgur.com/UqQ3jiH.jpg) | ![](https://i.imgur.com/kyKP8yX.jpg)  | ![](https://i.imgur.com/pwKzO6F.jpg) | 
| -------- | -------- | -------- |


![](https://i.imgur.com/YxxGmB9.gif)


Same builder could be used for making collector displays for wearables also
![](https://i.imgur.com/dHwBleJ.jpg)

![](https://i.imgur.com/1pwqUzx.gif)

![](https://i.imgur.com/ENkdMQQ.gif)

**Dev Log 3: 8-2-22**

https://www.youtube.com/watch?v=ViIMCvgmOUM

{%youtube ViIMCvgmOUM %}

**Dev Log 4: 8-16-22**

https://www.youtube.com/watch?v=I5uhAtCRXOw

{%youtube I5uhAtCRXOw %}


---

### MetaFactory

![](https://i.imgur.com/QL1NAen.png)


![](https://i.imgur.com/twgIr9L.png)

**Current base meshes**

![](https://i.imgur.com/V5BPWpr.png)
![](https://i.imgur.com/wXC7PBB.png)
![](https://i.imgur.com/o7QFkID.png)


### Webaverse

- https://hackmd.io/@xr/avatarlod
- https://github.com/avaer/avatar-asset-pipeline
- https://github.com/webaverse/app/blob/master/avatar-spriter.js

inventory of items (could unbundle?)
![](https://i.imgur.com/czUbG8a.jpg)

animated pfp version (threejs app?)
![](https://i.imgur.com/EHlkxra.png)

doom sprite version
![](https://i.imgur.com/0mlbEvD.png)

trading card version
![](https://i.imgur.com/K9FyIEk.png)


- Inventory + attachable wearables
- View with vehicles / pets
- High quality VRM support
- Optimized GLB
- Doom spritesheet
- 2D PFP (png/mp4)
- Trading card game design
- NPC / AI

---

### Wearable Packs

- https://api.babby.xyz/metadata/1642

cc0
![](https://i.imgur.com/V3wrXlS.png)

From Babbys 1-50
![](https://i.imgur.com/zvzOi0v.jpg)

Uncanny Alley assets

![](https://i.gyazo.com/cbcbceed493e9cafdf0a406de3f52f9b.gif)

![](https://i.imgur.com/m86Po1q.png)

---


## Closed / Non-free


### Meta

Prada, Balenciaga and Thom Browne partnered with Meta, more on the way apparently.

![](https://i.imgur.com/xyo8cbu.jpg)

> Luxury fashion houses are increasingly partnering with technology companies to create branded digital garments. Last year, Fortnite introduced **Balenciaga** skins so players could purchase garments like a branded hoodie for their in-game characters. In Roblox, players can visit **Gucci** Town, complete with a garden featuring the brand’s logo and a virtual store.

Link: https://www.theverge.com/2022/6/17/23173128/meta-avatar-store-clothing-balenciaga-prada-thom-browne?utm_campaign=theverge&utm_content=chorus&utm_medium=social&utm_source=twitter

![](https://i.imgur.com/rCoLi1a.png)

Identity is the cornerstone of the open metaverse as it pertains to how we represent ourselves and what data we bring with us between platforms. Mark Zuckerberg seems intent on evolving their social graph / identity layer to on-chain systems. They have already announced a partnership with Polygon.

Link: https://www.facebook.com/4/posts/pfbid021Q1ZMJFWcXBvPcaqpLWgp3x5HTMD3vyVNbPB17BcuX6n1UmAKh7Kyv6dUb6oKP7Nl/?sfnsn=mo

It will be interesting to see how the ripple effects of a social media and VR tech giant affect the rest of the ecosystem by taking big steps into web3.

### MetaHuman

- https://www.unrealengine.com/en-US/metahuman
- https://docs.metahuman.unrealengine.com/en-US/overview/
    - [Using Mesh to MetaHuman in UE | Unreal Engine](https://www.youtube.com/watch?v=xOVyme4TFZw)
    - [Making Realistic Digital Humans with MetaHuman Creator | Unreal Engine
    ](https://www.youtube.com/watch?v=PEYT1IPX0wg)

![](https://i.imgur.com/NtHMCqt.jpg)

> MetaHuman Creator is a free, cloud-streamed tool you can use to create your own digital humans in an intuitive, easy-to-learn environment. Using MetaHuman Creator, you can customize your digital avatar's hairstyle, facial features, height, body proportions, and more.

![](https://i.imgur.com/lWNwS75.gif)

---

### Genies

- https://venturebeat.com/games/genies-raises-150m-at-over-1b-valuation-for-metaverse-avatars/
- https://genies.com/


![](https://ph-files.imgix.net/87f4b9c3-c67a-4eb7-9c0e-260b951ac188.png?auto=format&fit=crop)



---

### Ready Player Me

- https://readyplayer.me/
    - https://docs.readyplayer.me/ready-player-me/

![](https://i.imgur.com/UGkTmW5.png)


Ready Player Me is the EZ mode standard for creating avatars that can be interoperable across tons of projects. They have over a thousand integrations via their SDK and you're allowed to download the GLB for your avatar. However, the licensing of the avatar is CC-BY NC, so you can't use it commercially.

![](https://i.imgur.com/SevGRlK.png)

This is the dashboard where you can select an avatar and view the differents app to take it into.

![](https://i.imgur.com/KCpwHao.png)

> We have conducted UX research on the avatar editor, to understand how we could create a layout that can be easily expanded in the future.
![](https://i.imgur.com/GAlcMQF.png)
https://twitter.com/readyplayerme/status/1551200788164349954/photo/1

Ready Player Me aren't all that super optimized, but devs are working on some big improvements to that. Currently they are ~9-12mb average.

![](https://i.imgur.com/fxhbXmk.png)


---

### VRoid Studio

- https://vroid.com/en/studio
- https://github.com/madjin/vrm-samples

My favorite program to design the avatar base mesh with. Get full rights to creations as a VRM file where you can encode the terms and ownership info into + preview animations. Millions of VRoids have been made. Has one of the biggest avatar economy ecosystems, check out https://booth.pm to see.

![](https://i.imgur.com/LLp66Xz.png)

VRoid studio is the only avatar builder program ability to create custom hair. It's as easy as drawing on paper. If you search vroid hair on booth, you can see some examples that people have made and sell. I bought some.

![](https://i.imgur.com/IKs55Kl.png)

One only has to know an image editor to create their own clothing for VRoids. This really lowers the barrier to entry as a creator. Cuts are transparency layers, and clothing can be overlayed.

![](https://i.imgur.com/F5y2g1C.png)

![](https://i.imgur.com/HFYFsHZ.png)

See https://github.com/madjin/vrm-samples

![](https://i.imgur.com/qIat5to.png)




---

### Character Creator

- https://www.reallusion.com/character-creator/cc-avatar.html

Paid program for high end looking avatars used by pro studios. It can generate an avatar based on a face picture.

![](https://i.imgur.com/lKlGRuS.png)

I was pleasantly surprised by the export stats, these are very usable in virtual worlds.

![](https://i.imgur.com/jwHkJ3L.png)

---

## Inspiration

- https://github.com/vladmandic/human-vrm
- https://github.com/google/mediapipe

![](https://i.imgur.com/CJhXFFb.png)
![](https://i.imgur.com/CxipPOZ.png)

---

## WebXR viewer

What if the avatar builder program has a webxr world in which you can preview your avatar with? What if the avatar customizer came with a personizable home space?

![](https://i.imgur.com/nlj3PCs.png)


---

### NeoRoid

- https://neoseast-japan.booth.pm/items/2562276
- https://www.youtube.com/watch?v=I38wxe-CUHg


**NeoRoid hub: https://www.youtube.com/watch?v=cvxqFEYkF1A**

NeoRoid hub is [CC0](https://creativecommons.org/publicdomain/zero/1.0/)

![](https://i.imgur.com/B2zdj1R.png)


![](https://i.imgur.com/ywHeD5X.png)

![](https://i.imgur.com/RzNef2u.png)

Bringing it into diff programs still needs work: https://twitter.com/dankvr/status/1439058671007371266




---

### AdWorld

- https://adworld.game/
- https://santangelo.notion.site/ADWORLD-WHITE-PAPER-d4724777866949928659f971c00d2d3c
- https://opensea.io/collection/adworld

![](https://i.imgur.com/Ap2d2Pt.png)

![](https://i.imgur.com/PUT1OxA.png)
See it in action: https://twitter.com/la53rshark/status/1524570277400694786

---

### Runescape creator

You'd be surprised how many people in crypto are ex-runescape people, especially the successful ones.

![](https://i.imgur.com/tcRCnAa.png)

![](https://i.imgur.com/KiyVKpS.png)

![](https://i.imgur.com/rwHOc1u.png)

### Loot Standard

- https://www.lootproject.com/#chapter2
- https://hackmd.io/@XR/lootwars

![](https://i.imgur.com/Jji60b8.png)


---


## Enhancement / Degradation

![](https://i.imgur.com/P0a8lDZ.jpg)

What if there was an avatar builder that could also export the loot version of something or 

![](https://i.imgur.com/VFKgg5A.gif)


#### Webaverse Trading Cards

- https://madjin.github.io/docs/docs/webaverse/items

![](https://i.imgur.com/f3nzfnP.jpg)

![](https://i.imgur.com/Ko0pgWs.png)

#### Hyperverse Trading cards


---

### Shopify Link

- https://shopify.engineering/how-we-built-shopify-party

![](https://i.imgur.com/LvAtrZK.png)
![](https://i.imgur.com/CkRg8VT.png)
![](https://i.imgur.com/8lZftPO.png)

### zepeto 

- https://zepeto.me/


![](https://i.imgur.com/8CPYtGd.jpg)
