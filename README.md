# Throne
A 3-D metaverse hosting platform based off of StruMML/RDS, Qt 6 (Qt3D), and licensed under GPL for a contiguous metaverse.

GOALS

To create a hostable and browsable web 3 experience using Qt3D and QWt libraries for UI/backend code and our research and aspirations into
using a standard definition markup language and a relocatable document system to maintain multiple client/server session data and provide live
delta information to standard definitions, preserving web-sites but using our conceptualization of RDS to provide for an interactive experience
in full 3-D immersion, whether viewed or interacted via keyboard (intially) but eventually through AR/VR as well. Our conceptualization and hopes
are to bring web 3 into something that can be eaisly integrated into old systems for maximal reusability and that by doing that we do not have to 
reinvent the wheel, entirely create new infrastructure, and can incorporate new technology such as photorealistic renders, new SPIR, and especially
blockchain technology which is already heavily dependent upon Javascript. By maintaing a document based format for the Meta-verse and the definitions,
requirements, and standards proposed by our research and implemented in this project, we can incorporate DeFi virtually seamlessly.
Enjoy and we welcome all future interests in our work!

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