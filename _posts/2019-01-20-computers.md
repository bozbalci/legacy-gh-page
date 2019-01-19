---
layout: post
title: "Computers"
date: 2019-01-20 00:00:00
---

I've spent most of my life around computers. Having chosen a career in computer science and software engineering, I assume that I will spend the majority of the rest of my life in the same way. In this post I tell the story of how I was introduced to computers, how my interests grew over the years, and how I ended up in this field.

# Early years

Our first home computer was bought in the early 2000s, and it ran Windows 98. It had a gigantic ergonomic keyboard designed by Microsoft. My mom told me that when I was three, I struck some keys on the keyboard and identified some letters as they appeared on the screen—that was how I learned the shape of some letters before ever holding a pencil. [^1]

Personal computing and Internet penetration was growing rapidly in Turkey in the early 2000s. One of the most memorable books of my childhood is "Bilgisayar Ansiklopedisi 2001", Turkish for "Computer Encyclopedia 2001". It was a huge, blue book filled with cheesy CGI images of zeroes and ones streaming through wires around the world and that really captured my attention when I couldn't read. I would look at pictures describing the Windows 98 UI, computer parts, screenshots from video games of the 90s. It was truly fascinating.

![Computer Encyclopedia 2001][encyclopedia-img]

{: .caption }
"Computer Encyclopedia 2001".

As soon as I learned to read, I began spending my evenings reading chapters from the encyclopedia and telling my dad, who would be working at the computer, about the things I had learned. I would sit on his lap and wait for him to finish his work so I could get on the computer and apply some of the things I learned. Mind you, I wasn't doing anything useful—my favorite activities were:

* playing around with the classic desktop applications located under the "Accessories" folder
* browsing system directories and trying to make sense of it all
* drawing sceneries in Paint
* trying to understand the rules of Minesweeper [^2]
* browsing the Control Panel. I loved the sense of power I felt when I was in there.
* breaking things on Windows Registry. I don't know how I even ended up in the registry.

About all you can do without Internet access as a six year old.

My favorite kind of programs back then were anti-virus software. I fondly remember the visuals of some anti-virus software, especially Spybot's "Search & Destroy". The concept of computers getting "sick" was very interesting to me and the terminology around the programs ("virus", "destroy", "immunize", "scan") and the nicknames given to malware was really getting me excited. That was about when I decided that I wanted to become a "computer guy", and design my own programs. I would sit down on Paint and draw fancy user interfaces, imagining how my programs would look if I ever learned how to actually produce them. I remember showing my dad an anti-virus program I "created". It was red, it was futuristic, and it was mine. That's one of the first things I remember being actually proud of.

There were monthly computer magazines we used to purchase regularly, and they issued a CD with each copy, containing trial versions of some new software, including video games. I used to install these video games to our computer without permission. My dad didn't like that, and told me to uninstall those games immediately. I was allowed to a maximum of two games, because having more than two games installed would slow down our computer, he said. But I didn't believe that found a workaround. I would install the game on an obscure location on the computer and removed all links to the game from the Start Menu, the Desktop, etc. to make sure that nobody would find them. That was my first computer *trick*. :p

After I started playing video games, my computer activities were mostly reduced to playing games—until we finally connected to the Internet and I was introduced to Flash.

## ~~Macromedia~~ Adobe Flash

Back in the day, Flash was really big. It was *the* platform for online multimedia content, long before the days of HTML5 and modern usage of other web technologies. Adobe announced in 2017 that they would declare Flash to be "end-of-life" in 2020. That's ten years after Steve Jobs' famous letter, ["Thoughts on Flash"][thoughts-on-flash] was published.

I had spent countless hours playing Flash games and watching animations created in Flash. My favorite websites on the internet were [Newgrounds][newgrounds] and [StickPage][stickpage].

My dad is in the online publishing and advertising industry, so he had obtained a copy of Macromedia Flash MX 2004 and it was installed on our computer. He's not a professional animator or programmer, but he wanted to learn his way around the program, gain some familiarity, so that he could communicate more clearly with the designers and perhaps perform some basic modifications before publishing without having to send it back to the designers.

One day I wake up to find this program installed on our computer and I was extremely excited to play around with it—perhaps I would create a Flash game like the ones I played! But alas, Flash MX 2004 was easily the most complicated program I had ever seen. Dozens of menus, unfamiliar UI elements, combined with my lacking English proficiency, it seemed like I would never be able to create anything with it.

Evenually I learned how to create simple animations by creating shapes and tweens. Once the concept of keyframe animation with the timeline *clicked* in my mind, I felt like I was the king of the world. But there was this something called "ActionScript 2.0" that seemed to appear everywhere: it's like there's a feature in this program that allows us to create *smart* things, but I couldn't even understand what it was.

I read some online tutorials on ActionScript, but my comprehension wasn't far beyond copying and pasting code around. **My virgin mind simply didn't accept the fact that I would have to write code in order to create programs.** My father had a collection of Flash tutorial videos from Lynda. He shared them with me, and I ambitiously watched every single video, but I didn't understand English: none of it made any sense to me, except I learned some UI shortcuts.

I remember from one those videos the instructor mentioning some `nQuantity` while writing ActionScript code. I replicated what he did on my computer, while thinking how strange of a word "nquantity" is, and how strange the capitalization was. I only realized seven years after the fact that it's just the [Hungarian notation][hungarian] for a number.

In many years, I developed a variety of Flash skills. I mostly used Flash as a vector drawing program, sometimes using its animation and multimedia capabilities (embedding video and audio) and rarely some interactive (very basic) Flash applications. This was very important to me, as it was my first coding experience at the age of nine.

## Grand Theft Auto: San Andreas

I am a huge GTA series fan. I've played (and fully completed) every game in the franchise since Grand Theft Auto III. I still play the classic games on my mobile devices when I find the time, and follow the speedrunning community closely. Among GTAs, the dearest to me is *Grand Theft Auto: San Andreas*.

The GTA modding community is among the most prolific communities found in video games. Two of the most significant modifications to the game are [_SA-MP_][samp] (San Andreas Multiplayer) and [_MTA:SA_][mtasa] (Multi Theft Auto: San Andreas).

Both of them are multiplayer extensions to GTA:SA, which is a proprietary commercial single-player PC game. Both of these mods are an incredible work of reverse engineering. They both work in the same way, through code injection and hooking techniques; leaving original game files unchanged. The multiplayer game engine adds networking and GUI rendering functionalities to the original game and exposes GTA-specific functionality through a scripting language. In SA-MP, this scripting language is [PAWN][pawn]. In MTA:SA, it is Lua.

My multi-player GTA:SA adventure initially took place in the SA-MP community. There was an obscure scene of competitive SA-MP players who liked to play on a genre of gamemodes called A/D (attack & defense). Those gamemodes were large PAWN projects and they added a lot of features not found in the original game. I founded my own clan (team) in 2008 and recruited more than 30 players. We were a force, except we didn't have our home server where we would host our own code and practice like other clans did.

In advance of getting a dedicated SA-MP server for our clan, I set out to write my own version of an A/D script. In my second foray into coding, I took some open-source examples and began adding some simple features tailored for our clan. I implemented a training mode where you would get random weapons on every respawn, and you would respawn much faster after dying. This was the first time I had created something useful out of the code I had written, but it wasn't a marvelous achievement as I had done it without having a clear understanding of what was going on.

After about four years spent in competitive SA-MP, I retired from the scene and moved on to MTA:SA, to embark on a new adventure: online role-playing. Online role-playing was one of the most valuable experiences I have had on the Internet, and it too contributed to my computer skills in a way.

### MTA

MTA is similar to SA-MP in many ways, but it is better: it's open source, more stable, has a lot more features, and it uses Lua (a much more popular language compared to PAWN) for scripting.

That's why a lot of the better gamemodes developed for the multiplayer GTA experience was found in MTA. It was easier to develop larger-scale, more complex gamemodes in Lua. The role-playing gamemode is most probably the most complex project among all gamemodes. The most popular type of RP is set on the fictional San Andreas. People create their characters and the rest is just like in real life. The GTA:SA game engine is used for the visuals and gameplay, while player actions and speech is represented in text. There is a very rich GUI where players can interact with their inventory, objects in the world, and NPCs. There is a very versatile set of commands allowed to be ran by admins, who assume the role of the gamemaster often found in traditional tabletop RPGs. 

I was part of the largest and most widely known role-playing community in MTA, it was called *Valhalla Gaming* throughout its existence. It was later renamed to *Root Gaming* and then it dissolved. The source code for the gamemode was leaked many times, and this has caused a number of lower-quality successors to Root Gaming. In due time, the roleplaying community was rebuilt in newer communities, namely *United Gaming* and finally *Owl Gaming*. I've always found it strange that all of these communities just had to have "Gaming" in their names.

When I first got into the roleplaying scene, I had very limited English vocabulary and did not understand what roleplaying was supposed to be. In almost 10 years of roleplaying, I made friends all around the world, attained English proficiency, learned a lot of things about law enforcement and organized crime (because of the kind of roleplay I was doing) and learned Lua and MySQL. Near the end of my presence in the MTA roleplaying community, I became an admin and scripter, contributing to the game that I loved to play every day.

## High school

To be written.

[^1]: I doubt this story, but I like to think that it's true because it allows me to say that I've been typing before I could write. :p
[^2]: I finally figured out how to play Minesweeper about 10 years later in high school.

[encyclopedia-img]: /images/bilgisayar-ansiklopedisi.png
{: .third}

[thoughts-on-flash]: https://www.apple.com/hotnews/thoughts-on-flash/
[newgrounds]: https://www.newgrounds.com/
[stickpage]: http://www.stickpage.com/
[hungarian]: https://en.wikipedia.org/wiki/Hungarian_notation
[samp]: https://www.sa-mp.com/
[mtasa]: https://www.sa-mp.com/
[pawn]: https://www.compuphase.com/pawn/pawn.htm
