# MDA

Hello! The purpose of the MetaDiscourse Analysis (MDA) library is to develop and provide access to tools for local dictionary Meta Discourse Analysis of text. This library focues on studying Discourse marker usage and distribution in a wide variety of discourse genre, not limited to (1) In-classroom discourse such as lectures, student written reflections, verbal presentations, (2) Entrepreneurial discourse such as pitches, (3) Political discourse such as presidential debates and op-eds.

## Why is this package relevant and unique?

Metadiscourse is embedded in everyday communication actions.  Based on Hyland's taxonomy metadiscourse are those unary or compound words and phrases that allow a person to take an authorial stance.  In other words, metadiscourse is not _what_ one says, but **how** one says it.

There are no open source python packages for metadiscourse analysis.  Our package not only provides a dictionary for this analysis, but also provides a quantitative analysis template through the ecosystem of other open source packages.  This package will further be augmented through LLM-driven rhetorical move identification.

## Metadiscourse Markers
Discourse markers are words used to link, describe, and organize ideas in written and verabal discourse. In broad terms, they are organized into ten categories: Code Gloss, Endorphics, Evidentials, Framemarkers, Transition, Attitude markers, Emphatics, Person Markers, Engagement, and Hedges. While there are words that are most commonly used in a specific category, they may be used in multiple categories, or their specific usage may be best determined based on context. 

### Code Gloss
These markers are used to adjust the meaning of a phrase or idea. 
Examples include: i.e., (for) instance, defined (as)
### Endophorics
These markers are used to point to additional information or evidence, after it has been stated that evidence exists. 
Examples include: "Chapter", "Figure", "Table"
### Evidentials
These markers relate support for an idea or concept in a general form, as opposed to endorphics.
Examples include: "Cite", "Quote", "According" (to)
### Framemarkers
These markers indicate that the discourse is moving through stages. There are four types of Frame markers: Sequencing, Announce Goals, Lables, and Shift Topics. 
#### Announce Goals
These markers are used as an explaination of the goal or purpose of the discourse is. 
Examples include: "this", "aim", "focus"
#### Sequencing
These markers are used to demonstrate the stage or order of a content section in discourse.
Examples include: "Chapter", "Section", "Finally"
#### Lables
Lable markers are used to end a segment or thought in discourse, and often are used to introduce the last portion of a statement. 
Examples include: "Conclusion", "Summary", "Moment"
#### Shift Topics
A Shift Topics discourse marker is used to start or end sections of discourse. 
Examples include: "Return", "Regard", "Move"
### Transition
Transitional markers demonstrate movement from one sentence or thought to another, often showing a contrast between the two. 
Examples include: "Accordingly", "Additionally", "Contrast"
### Attitude Markers
Attitude markers show ones opinion or attitude in discourse.
Examples include: "Admittedly", "Dissappointed", "Disagree"
### Emphatics
Emphatics are used to demonstrate ones opinion or perspective on a topic, and often are used towards the end of a thought.
Examples include: "Actually", "Always", "Must"
### Person Markers
Person markers are used to identify the main person(s) the current thought is regarding.
Examples include: "I", "Me", "We", "They"
### Engagement
As you may have guessed, Engagement markers are elements of dicourse used to draw readers or listeners into the discourse, or to negotiate with them. 
Examples include: "Reader", "Assume", "Ensure"
### Hedges
Hedges are markers used to soften a statement or show doubt or lack of certainty. 
Examples include: "Appears", "May", "Indicates"


## MetaDiscourseAnalysis Class

This is  the default class for the MDA library. The class allows users to import text and run analysis on it, to check the relative percentage of dicourse markers.
When a class object is instantiated a homebrewed dictionary of discourse markers is initialized for each marker type. These are used to identify markers in the text and categorize them. Future editions may include ability to adjust the dictionary content, as well as identify unique markers used in the text. 

### Class Functions
Here is a short overview of the current functions. If you have suggestions on improvements or additional program features, please feel free to let us know and become a contributor!

#### Authorial_stance(Text) 
Requires text input. This processes the text, counts discourse markers in each category,

**Returns:** Text length, total number of Interactional markers and total number of interactive markers.

#### Log(Text)
Returns a printed output of the text stripped of white space. Used during preprocessing. 
## Package Dependencies
**Numpy**  - This assists in the mathematical analysis of the processed text.
**Pandas** - This assists in processing, storing, and manipulating the text
**String** - Builtin python module used for string manipulation
**Gensim** - Used for text processing.
**tqdm**   - Utilized to show progress bar during computation. 
**os**     - Builtin package used to import files. 
**plotly** - The "Express" extension is utilized for fast visulization of the function results. 

#### Upcoming Features
In the next package iteration we are planning to improve the data visulization ability through additional default graphs and a dedicated graphing function. Additional investigative functions to explore change in marker usage over time, or as the moves from beginning to end will be added as well. 

## How to Get Involved

If you find this library useful and would like to add your own ideas to it, we would love to work with you! To get involved, Read over the contributor code of conduct and contact dnaneet@mtu.edu to join the mailing list and get started.
