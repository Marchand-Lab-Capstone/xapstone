# User Stories - 2/15/
The following stories are designed with the intention of aiding our understanding of what
our end goal should be, as well as what we may want our design critera and use cases are.

---
Case 1:
User: Dr. J. Eggbert
Dr. Eggbert is a researcher and biotech researcher, who is trying to repurpose his
existing hardware to help him with his development of atypical DNA sequences, for the future
purpose of in-vitro xenobiology. His lab partner, Dr. K. Vantas,
has sent him a handful of dna samples that Dr. Eggbert has no information on. Eggbert knows that
his existing nanopore sequencing technology isn't inherently limited to standard bases, but does not have the
time to develop his own tool to check if the samples from Vantas are modified or not, and due to
Dr. Vantas being busy, does not want to bother him about it. Eggbert is not particulray knowlegable
about software tools. 

Overview:
- He wants something that is capable of interpreting existing data
- He wants something that is relatively unobtrusive/not time consuming
- He wants something that can tell you if a sequence contains XNA or not
- He may want a somewhat friendly user interface.

---
Case 2:
User: J. Sumabat (Master's Student Verson)
Jayson is the primary user of this software and will be implementing this into a larger overall de novo basecalling pipeline for any modified/synethic bases. He is trying to develop this tool in a way that can cover a wide span of users, from academia to the growing xenobiology market. He does not particularly care about having a GUI but isn't opposed to having one. Jayson has experience with command line, software tools, and the underlying biological principles but wants this intermediate tool to be easily applied to a larger pipeline. Lastly, he wants code that is well documented because he will have to recall this information a year from now for a thesis defense. 

Overview: 
- He wants something that can be used in tandem with other programs
- Easy to understand but good documentation. 
- Generalizability for any modified bases 

--
Case 3:
User: York Vega 
York is an undergraduate student who has gotten in to researching biology and was tasked by her
PI with the identification of possible xenonucleobase locations in a sequence she has been given.
She doesn't have any experience with code or data science, she only knows how to drag and drop files, and maybe enter a command into a command line. She wants an output sequence that has a simple marker of areas of interest. 

Overview:
- She would like to take the simplest route possible
- She is likely to input something incorrectly due to inexperience
- She wants a simple, human-readable output
- The data she has is a hectic compilation and wants it to be distilled down
