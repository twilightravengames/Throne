# Throne
A 3-D metaverse hosting platform based off of StruMML/RDS, Qt 6 (Qt3D), and licensed under GPL for a seamless metaverse.

WHY A SEAMLESS METAVERSE?

Companies are currently struggling and finding themselves failing to create private metaverses with incompatible technology and somehow link them together. It reminds me of the early days of the Internet, before the first HTML document was hosted, hyperlinks were not a thing, and there was no interconnection between websites. Before the world wide web. If you like history, you can look back to see the hosting of the first HTML document was the beginning of the WWW. We think the same approach can be made with Metaverse technologies. 

Our vision is to have a Metaverse so vast it is as large as our global Internet today. But we don't think one company can do it on their own. We feel we need to build on the infrastructure of web 2, just as the original world wide web was built upon previous infrastructure. We don't expect to make any money off of our ideas, we'd like to, but we believe in a structure that will create a more powerful Internet in the form of a Metaverse in the future. We aren't overly ambitious, we believe it will take a lot of time and investment. But we think our approach will work better than what is being tried right now. It is more practical and is based on foundations, not speculation. Our vision would make the worlds seamless, dwarf games like World of Warcraft or Fortnite in size. Even be able to be holding a meeting in your virtual office and then battling monsters on a foreign island on your lunchbreak, all in a seamless environment. Is this really more silly or far off than coloinizing Mars or shooting asteroids that might collide with Earth out of the way?

It would start with laptops and PCs and cheaper hardware, a browsable Internet, and gradually incorporate VR hardware as prices drop and technology is advanced. Concepts that are only distant and seem out of reach right now like virtual real estate, improvements to remote work that would not involve tireless zoom meetings where you only see a person's head but see their body in the form they like and gesturing the way they want to gesture. The kinds of things we dream of when we watch the cool technology in movies like "Ready, Player One." 

We believe this is the ultimate goal of all companies investing in Metaverse technology, Avatar technology, and Web 3 as well. We only believe we have a more practical way to start and that baby steps are better than speculative, untested, leaps and bounds. 

GENERAL EXPLANATION AND HOW WE THINK IT WILL WORK

THe goal is to create a hostable and browsable web 3 experience starting with building on web 2.0 infrastructure. Qt is our choice for primary UI and rendering because of its ease of use, continuing development, increasing popularity, internal 3D API, and simple to use UI components. Qt is our choice for our so-called browser into the Metaverse. This is not a set in stone thing, it is what we think is the right choice right now. The "Alliance" project is like a web 2.0 browser but instead it is a portal for PCs to view Metaverse "pages" like they would view a level in a game. The pages instead of being viewed as 2D pages are viewed in 3D, but for all intents and purposes still exist in a format like HTML docs. These 3D level "HTML" docs that act like levels in a game are what I call the StruMML docs. The second type of docucment is RDS. RDS documents are shorter, less detailed. They make it so the Metaverse levels can be updated in real-time. They contain the changes in a document form. The changes are communicated through RDS documents between the server and all the browsers connected to it. This allows us to make every level dynamic, constantly undergoing change.

The "Throne" project is just the server side project for "Alliance."

BUT WHAT ABOUT SEAMLESSNESS?

It may appear that this will not make a seamless user experience. We would have a bunch of little worlds all scattered around defined by tiny web pages and we would be jumping between them like we do web pages. This is not the case. Each "level" or as I like to call them, "sectors" would behave kind of like in the classic game DOOM, which I borrowed the terminology from. A sector would define a portion of the seamless Metaverse but there would be boundaries to each sector. Instead of jumping from world to world like in the game Portal Knights, or from one giant world to another giant world like in Fortnite, the sectors would use level of distance (LOD). This means that when something is out of sight, that is how we would define the boundaries of a sector. As we approach the boundaries, old data is discarded and new data about the boundary sectors is loaded.

HOW CAN WE MAKE WORLDS SEAMLESS? WE CAN'T FIT TOGETHER CIRCULAR WORLDS

This problem was brought up on the Ultima Online (SERV-UO) forums over two decades ago. The best solution was to use a honeycomb like boundary system for the sectors. 
Becuase we cannot fit spheres together seamlessly, the proposed solution to this problem was the most efficient structure in nature. Each secctor would have the boundaries of a honeycomb hexagonal cell. In plain english, the space in an individual part of a honeycomb. This is the most optimal shape in mathematics and for computation. Imagine if you are in the middle of the sector. All the sectors around you would be gathered in memory ahead of time, but not shown. As you appproach another sector, you can begin to see the surrounding sectors that are most closely adjacent to you. Say you move into one of these new sectors. Now the browser only has to worry about the sectors surrounding you that are directly adjacent to you, once again. It does not need to know about any of the other sectors in the Metaverse.

WHAT HAPPENS IF SOMEBODY HACKS/DAMAGES MY "METAVERSE" PAGE

This is again where the two file system comes into play. While the "StruMML", the HTML like documents, contain a definition or baseline for the Metaverse "page", the RDS documents are kept on the server and the browser. This means that at any time the owner of the website (using this term loosely) can go and reset back to the baseline. 

WHAT ROLE WOULD HYPERLINKS INVOLVE?

Instead of jumping from page to page like we do now, we would transition from Metaverse page to Metaverse page by moving across sector boundaries. There is always the option to create some sort of portal to jump from one distant world to another. In the Infiniverse/Multiverse on the Oculus Quest the ideas of public transportation to transport from location to location has been explored. 

WHAT ROLE DOES A WEBSITE NOW PLAY?

A website is now not only a web address but as has been suggested by some Metaverse proponents, more like a physical address. The web address would guide you to a collection of pages, just as it does now. But these colletions of pages would be linked together by boundaries in their respective pages (sectors). The role of a website now changes a little. It is no longer the responsibility of a website to provide documents, but rather, a portion of the virtual world. We already live in a partially virtual world, this transition makes sense to us. 


CONCLUSION

This is our vision so far. We welcome comments, suggestions, inquiries, investments, or just plain retweets and spreading the word. This is a simple solution for a complicated technology. We find that in most cases in life, simple solutions for complicated things work.



2022-10-16 9:34 PM EDT 

This is the initial posting of the repository for the Throne StruMML/RDS web-server (hosting application may be more appropriate)
to the public. This repository includes ongoing research that is WIP by Twilight Raven Games LLC under GPL 3.0 that is included in the docx
WOrd documents included for download with this repository. 

CHANGELOG
=========


It has been decided that Throne will use Pixar's USD file format as part of it's backend and the StruMML/RDS document standards have been grouped together into a more common standard, name, CMV - Contiguous Meta-Verse

DEPENDENCIES
============
Consumes CMV-SDK
Consumes nginx (For fast hosting over http of StruMML and RDS documents - standardized xml )
Consumes Qt6
Consumes tinyxml2 (For xml parsing)
