#GSoC 2015 proposal for KDE


 



#Port of Gcompris to QtQuick

 
 
 
 

 

##Abstract

 

GCompris is about learning through play . While being interesting to play, every activity should also enhance the knowledge of the children. I propose to extend the GCompris activities section by adding computer science activities and porting the lang activity.

 

Computer programming is incredibly empowering skill to learn. The programmers of tomorrow are the wizards of the future. In this section there will be some interactive games for kids to that will build their logics and make them familiar to world of computer programming.

 

Language learning is another very important need for every language we need better vocabulary to express ourselves. Also reading/writing section is the area where large amount of work for porting is to be done.

 

 

##Motivation

 

GCompris is a complete package for any child to explore the whole world of learning. Keeping in track with this era, It is highly likely to introduce kids to basic computer science methodologies. Its inspiring to see a smile on the face of kids ( including my cousins ) while playing GCompris math activities, while in real life they find math the toughest. I would like to make it more complete and enjoyable experience for learning.

 

####Computer learning activities :

 

Up until a few decades ago, people shared ideas through the written word. If you had the ability to write, you had the ability to create change. Today writing is not nearly as effective in changing behavior as manipulating ( or leveraging ) the digital medium. To know how to program is to understand, to build, and to change. For the leaders of tomorrow, there is perhaps no skill as important as learning to program.

 

Learning how to program is like learning any other language. The difference, of course, is that programming can be much more powerful. With just a computer, kids can use the skills they learn to build something that might change the world. It stretches your mind and helps you think better, creates a way of thinking about things that I think is helpful in all domains.

 

####Lang Activity :

 

Language learning in particular require long and complex process to learn. Overall, reading methods must be resilient to the vicissitudes of implementation. Books alone are not sufficient to keep children's interested in languages. A game which will be fun to play for them can be a good early start for learning for every children.

 

 
 
 

##Proposal:

 

To create six activities touching two sections of the GCompris.

activities

####1) Language Learning Activities

 

We are creating activities that will involve a child completely. It is proven method to learn better when we involve more senses rather than just reading (that is seeing the word). In our activity the child will look at the picture of object, hear the pronunciation of it, and will learn by speaking it aloud.

 

Also known as lang activities in gcompris legacy version. I will port the all subparts of it namely lang-nature, lang-object, lang-other and lang-people. We can call all these collectively lang activities.first we prompt the user to choose a category from nature, vegetable or actions. And after it they need to choose difficulty i.e. begginer vegetables, intermediate vegetables, Expert vegetables.

 

The start menu will incorporate a visual feedback for the learning. A progress bar showing the percentage of words correctly learned in each category and each difficulty level of respective category. Correctly learned means correct answer to all the quiz for the word. It will be updated in real time and shown to user while playing. This is a way of giving small rewards at every small footsteps.

 

#####1. Intro to Words

 

The category of the word i.e. vegetables, animals as the heading at the top. The picture and the spelling of the word. The word will be pronounced also. And there will be functionality to repeat the pronunciation. By this activity we expose the child to a new set of vocabulary as par their experience level. It will be immediately followed by a set of mini games for the learnt words. There will be maximum 12 words at a time.

intro to word

 

 

#####2. Quiz mini games

 

The mini games are to test the kids recognizance power for the particular word by looking at the Image/text and hearing the sound. This will be based on same set of words which we learnt during the intro to words(first part). It is divided in three parts

 

 

Voice + Text & Image + Text : Word is shown in text format and also pronounced. Answer options will be displayed as image and text.

 

######mini game 1

Voice & Image + Text : Word is only pronounced for the question. Answer options will be displayed as Image + text only.

######mini game 2

Voice & Image : Word is only pronounced for the question. Answer option are displayed as only Image.

######mini game 3

These screenshots are taken from old lang.

#####3. Spell it!

 

The last mini game is to empower them to write and remember the spelling of the word displayed in picture. The hind is displayed letter by letter if the answer is incorrect. After completing this level the user will proceed to another set of words.

spell it

 

####Computer science Activities

 

These are the new activities i am proposing to do under computer science activities. 

#####4. Maze:

 

This activity will focus on making the kids learn algorithmically and write simple programming constructs. We will make it simple for them. They need to write just letters according to our instruction. The instructions will be listed for picking up by the user. Also these statements will be localized.

 

Programming constructs will be provided in form of a list consisting of simple statements like turnLeft, turnRight, moveForward etc. by picking them and arranging them in order the child will try to solve the maze puzzle and lead tux towards its home.

 


 

#####5. Bird

 

This activity introduces concept of argument to a function. It introduces new functions such as rotate and by picking rotate they will be prompted to pick an angle by which to rotate. This will enable the kid to understand the value of using any instruction and introducing the variation which he can create.



 

#####6. Code to Draw

 

Code to draw is an activity to draw simple and complex shapes such as square, pentagon and star. The kid walks over any path and stamps the path with the given color such that after reaching the end. It creates the desired shape. It includes one new function that is draw. Thus the kid learns the function of usign a function when needed and create patterns like linear or alternate.




##Implementation 

I will use Qt creator for development and openclipart and inkscape/gimp for designing the user interface and logos. As i have already ported an activity i am familiar with the GCompris codebase by now.

 

##Time line

 

####Activity wise time line

 

######Lang Activity

Intro to word : week 1

Quiz mini games : week 2-3

Spell it : week 4

######Computer science Activities

Maze : week 5-6

Bird : week 7-8

Code to Draw : week 9-10

 

####Week wise timeline

 

###27 April – 24 May ( Community bonding period )

 

Further discuss the activity ideas with mentors.

Designing icons and logos for activities using Inkscape and openclipart.

Discuss and create detailed wire frames for user interface of every activity.

Study api for Lang activities.

 

###25 May – 26 June ( Work period )  


####Week 1

Start Coding !

Complete the Intro word sub activity. Some work already done by me.

 

####Week 2 

Designing quiz games.

Coding for quiz games all 3 mini games in this week.

Complete the second activity.

Document the work.

 

####Week 3

Design UI for Spell It sub activity.

Build up algorithm for the activity.

Implement the algorithm.

 

####Week 4

Create Visual feedback for Lang activity.

Connect the percentage of completion to different quizzes and spell it.

Completion of Lang Activity.

Optimize the code.

Document the work.

 

 

###26 June – 3 July ( Mid term evaluation)

 

Deliverable : complete Lang Activity containing all the three sub activities.

 

 

###3 July – 17 August ( Work period )

 
####Week 5 

Design UI for computer science Maze activity.

Design hard coded mazes.

 

####Week 6

Code the backend for the maze activity.

Implement the list of functions like moveForward, turnLeft.

Complete the maze activity.

Optimize the code.

Document the work.

 

####Week 7

Design UI for Bird Activity.

Design Levels and hurdles for the activity.

 

####Week 8

Implement the rotate function with a specific angle.

Completion of Bird activity.

Implement the list of functions like moveForward, turnLeft

Document the work.

 

####Week 9

Design UI for Code to Draw.

Design different levels and shapes to draw.

Optimize the algorithm and creating animations with states/transitions wherever applicable.

 

####Week 10

Javascript for the draw function using Canvas element.

Completion of the activity.

Optimize the code and design for smaller screens.

Document the work.

 

####18 August – 28 August ( Pencils down )

 

Testing & Debugging.

Final release.

 

####About me

 

Name : Siddhesh Suthar

Email : siddhesh.it@gmail.com

IRC nick : siddhism

Git url : https://github.com/siddhism

Location : Rajasthan, India

Timezone : +530 GMT

 

I am a final year student pursuing my bachelor of engineering and technology in Information Technology at Govt. Engineering college bikaner, Rajasthan Technical University, India. I am open source enthusiast and familiar with FOSS since more than one year now.

 

I have a working knowledge of Qt, qml, QtQuick development, python, java, android SDK, android application development. I am already well versed with community interactions/dynamics of OSS projects. I frequently use irc, mailing lists, version control systems such as git & host all my projects at [github](https://github.com/siddhism) hence I can start early with the coding. I take summer of code as an opportunity to get engaged with KDE community as a contributor and continue this association even after GSoC.

 

My open source contribution to Gcompris, the pull request which got merged can be found [here](https://github.com/bdoin/GCompris-qt/pull/64). I created an activity for introduction to gravity concept.

 

Also, I am a member of Linux User group Bikaner (lugb) and have contributed in organizing FOSS event RajasFoss at our college campus. I would love to be contacted if any part of this project proposal is not clear to you. Thank you for considering this project proposal and for your time.

 
