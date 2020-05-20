
# ROADMAP: Family Recipes Version 0.0.00
Future expansions are considered in this file. 
Their presence is not a promise that they'll exist, but rather this file serves as an
early outline of features this project hopes to add, as well as changes in directions


The format is adapted from [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
It wont adhere perfectly, but it's a start. 


Dates follow YYYY-MM-DD format






## [0.0.00] Family Recipes 2020-XX-XX
In Progress
### Contributors
Keith Murray

email: kmurrayis@gmail.com |
twitter: [@keithTheEE](https://twitter.com/keithTheEE) |
github: [CrakeNotSnowman](https://github.com/CrakeNotSnowman)


Ian Finley

github: [ianfinley89](https://github.com/ianfinley89)


Unless otherwise noted, all changes by @kmurrayis or @ianfinley89


### Short Term Roadmap


KM Short Terms
Figure out a virtual enviornment and see how difficult it is to get known dependancies up and running between pcs

Goals:
 - Set up dev branch
 - Python 3.x (I'm using 7 but with a ve we can adjust as needed)
 - moviepy or similar ffmpeg wrapper library (I like movie py because it's easy once it's installed, but after a learning curve, I'm sure any library is)
 - YOLOv3, (Or, I guess, any similar object detection)
 - PyTorch Something or other (Probably a later requirement but an 'early' sort of later requirement)
 - A helloworld test for each library to make sure it runs in the tests directory

Past that, maybe a simple hello world which takes a video, extracts x frames, passes the frames to yolo, and returns a list of detected objects. That seems like a good marker to move to v0.0.01, and we can expand goals then I'd reckon.

 
#### Add
#### Change
#### Deprecate
#### Remove
#### Fix
#### Security
#### Consider 
#### Testing


 
---

### General to Long Term Expansion

### Main
### Utils
### OTHER
KM

Program outline
Presuming the input to the program is a video, or collection of videos of someone cooking

- main.py will take in a path to the video, or directory of ordered videos
 - the video will be opened with [Some module like moviepy]
 - Pull out the audio so any speech can be added to a stt program 
   - The audio all probably contains signs of actions: chopping noise, stirring, etc. This will probably be a late feature extraction, but might be worth considering
 - Initalize an empty list of 'items': this will get populated then pruned to be used as the ingredients list 
 - Since each line of a recipe card is sorta equavilent to a 'scene', split the video into scenes, where sort of one operation, or class of opperations is done. This will be handwavy. 
   - Use some form of NRE + video object detection to establish what's present, and then some form of action extraction to figure out the order of opperations. This is a bit vauger but kinda similar to the event twitter bot which tries to extract event specifics from a block of tweets. There might be crosss applications/functions which are useful in both programs. 
   - There's a very real likelyhood that we can build out some form of knowledge graph from the video, the use a ... topological structure (ok probably not that), or probabilitic structure and feed the graph to .. probably a cnn, to fill out the recipe card. When all you've got is a hammer everything looks like a nail, and I'm thinking of it as a question answering system, so the solutions to this problem that I'm thinking of fits that structure. Basically an empty recipe card is what we're starting with, the question is 'given this knowledge graph, what is the recipe?' the corpus to search for the answer is the video, and the named entites and order of opperations are what we extract to serve the answer. 




#### Topics to explore
- Federated Learning
- Meta learning
- Few-shot Learning
### Tests 
### Docs

