# Piction

This is an [unplugged activity](https://csunplugged.org/) about
pictures and languages. This game can be played either at science forums
or in class settings. 

- Age range: tested with 9 years-old pupils and with 15 years-oldstudents.
- Duration: about 45mn
- Material: 
  - Pencils (one per participant)
  - Two printouts:
    - a [model](models.svg) sheet per group, cut in 4 parts along the lines;
    - a few [blank models](blanks.svg) sheets, cut in 9 parts along the lines.
      You can use free paper or slates instead of blank sheets if you wish.
- Activity integration: can be played alone, or along (before or after) the
  [image representation](https://classic.csunplugged.org/image-representation/)
  of CS unplug (see conclusion below).

### Introduction phase

Participants are grouped by small groups (typically 3 to 5 people). 

In each group one participant (called the narrator) is given the part
of the model sheet that has a big A on it while the others (the
drawers) get a part of the blank sheet and a pencil.

### First active phase: Drawings the A sheet

- Setting: small groups (3 to 5)
- Role of the participants: describe and draw flags
- Role of the animator: move from group to group
  - Ensure that all groups understood the game. 
  - Ensure that the narrator role is well shared between participants. 
  - Ensure that the noise level remains bearable.
- Possible scaffolding (for the slow groups): the narrator should look
  at what the drawers are doing to get some feedback on what they
  understand of the explanations.
- Possible extension (for the fast groups): more flags to draw (?)
- Duration: about 10mn

In each group, the narrator is asked to pick on of the flags in the
sheet, and describe it to the team mates. When done, the group
compares the original flag to all drawings. The closer the better.

Another participant is chosen as narrator, get the A sheet with the
models, picks another flag and describe it to the group. 

If everything goes well, the groups will have difficulties getting the
drawing resemble to the models, and this is exactly where we want to
go. It is a good idea to end this phase before the arguments get too
loud :)

### First wrap-up

- Duration: about 5mn

The animator speaks with the whole class, summarizing how the previous
phase went. Once agreeing with the class that there is a communication
issue ("they don't understand a thing!" vs. "you just talk
gibberish!"), the model sheet of vocabulary is given to the groups. It
contains indications on how to precisely describe the flags. Then,
every groups go back to the activity, with this new help.

### Second active phase: Drawings with a method

- Setting: small groups (same as before)
- Role of the participants: describe and draw flags with this new vocabulary
- Role of the animator: as before + monitors the advance of groups, and give
  sheets B and C when the previous sheets are exhausted by the groups. 
- Duration: about 20mn

The groups can try the vocabulary on the remaining flags, switching
narrator between each flag. The sheet A is made very simple with this
provided vocabulary, and the sheet B should be of the appropriate
difficulty. The twist is that the provided vocabulary is not
sufficient to describe all flags of the sheet C, forcing the groups to
come up with their own vocabulary extensions.

### Final wrap-up

- Duration: 5mn

The animator collects the participants' feelings about how it went
with the new vocabulary. A discussion may occur on the limits
experienced on the third sheet, and how each group overcomed them.

No such activity shall finish without a discussion with the class
about the connexion to the CS field. The animator may first ask the
class about their feelings on this connexion, and discuss rapidely the
collected answers. There is several links to CS, detailed below.

# That's Computer Science!

- Duration: 5mn

We organize the discussion using the four axes Language,
Information/Data, Algorithm and Machine that is are common in the
French literature of CSE, but other referential could be used.

### Language (\*\*: very relevant)

This activity was invented to highlight the concept of computer
Language. The goal is here to communicate effectively the exact
description of different patterns (which are here flags): the
description must be sufficiently precise for the drawer to 
redraw it faithfully.

During the activity, participants understand the need to define and
use a specific language adapted to the task. It is necessary to define
the authorized words and expressions (the *syntax* of the language), as
well as their meaning (the *semantics* of the language).

This activity also allows explore different language characteristics. 

First of all, the *expressivness* of a language determines the set of
objects that the language can describe. In the activity, the sheet B
provides patterns that are easy to describe with the language of the
vocabulary sheet, but the sheet C proposes patterns that show the
limits of this language. We can thus measure the expressivity of the
language by the number of flags that can be described.

In general, a language can not describe everything. For example, a
language describing line segments will not allow not to describe a
circle. We can always extend a language to make more expressive by
making it more complex. It remains formally impossible to come up with
a language that describes itself entirely.

Then, the definition of a language raises the question of its
*ambiguity*. This is a question related to the semantics (to the
meaning associated with the signs): The language is ambiguous if
several meanings can be associated to the same description. For
example, saying "cut the figure in two parts" is ambiguous if we do
not specify whether to do it vertically or horizontally, or if it is
not clear whether the parts should be same size or not.

A language that leaves room for ambiguities (like English) is more
suited to describe feelings or make poetry but it is not suitable for
communicating with the computer. This is one reasons why the notion of
language is paramount in computer science.

More precisely, when describing an algorithm for a computer to execute
it, we need a language that can be understood by this computer, such
as Python or Javascript. This is what we calls a programming language
(you write programs with them). This clarifies the difference between
an algorithm (here the description of the flag using an informal
english) and a program (the formal description using a pre-defined
precise language). The concepts of expressiveness and lack of
ambiguity are naturally essential in the development of a programming
language. Ambiguisty is particularly difficult to overcome for
computers. You could decide to react randomly to ambiguity, but it
would be little desirable if the programs responsible for the
deployment of car airbags would behave randomly.

### Information and Data (\*: relevant)

This activity can be used to discuss how an image could be represented
in memory (related to *Data*). It is easier if the class played the CS
unplug activity on bitmap represententation, but that remains possible
even if not.

Bitmap and vectorial representations of images are very complementary.
Once the idea of bitmap images is clear, the animator can explain how
bitmaps are badly suited to extra zooming while vector image never
loose in quality when zoomed in. A printout of a pixelized image helps
this discussion.

One can also discuss the image sizes with each representation to
discuss their relative efficiency. Vector images are clearly the best
option for these flags: you save memory size, with a better zooming
quality. To the opposite, storing the picture of a landscape is
probably difficult using a vector image (some could argue that
wavelets of jpg are related to vector image, but that's beyond the
scope of this activity. The animator should just remain careful on how
vectors are difficult to adapt to real images).

The pdf format, originally intended for printing documents, is mostly
vectorial even if it can also include bitmaps. The way to describe web
pages in HTML is rather close to a vector representation (you describe
what elements should appear where on the screen), just like file saves
of a word processor.

Optionally, you could also discuss more abstract ideas on *Information*
by reflecting on how the patterns were separated between the sheets A
and B. All of these patterns can be described with the proposed
language, but some of them are clearly more complex than others. How
could it be quantified? When given two flags, how would you decide
which one is more complex?

What we did while building this activity was to write down the
representation of each flag in our language, and sorting them
according to the length of the description: the longer the
description, the more complex the flag must be. This is however
disputable, because some of the flags on the sheet C could have been
placed on sheet B with a slightly different language. This leads to a
very profound question: given a flag what is the absolute minimal
amount of signs that you must use to represent it unambiguously? A
precise answer is far beyond the scope, but you can get a first
approximate answer on your computer: just zip that file, and see how
big the resulting archive is.

### Algorithm (.: not relevant)

There is no easy link between this activity and the concept of
Algorithm. Simply see the discussion in the Language section on the
difference between algorithms that are not necessarily formally set,
and programs, that must be unanbiguous to be usable by a computer.

### Machine (.: not relevant)

No visible link.
