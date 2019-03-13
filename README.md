# cpp_20Questions
A simple '20 questions' style game written in C++

Input/Output format for this program.

A tree of questions and answers is represented by multiple lines of
text. There will always be at least one line of text.

Each line represents one node in the tree. Each begins with either a
'Q' or an 'A', indicating whether the node is a Question node or an
Answer node, followed by one or more blank spaces, followed by the
text of the question or answer. The text of a question or answer
begins with the first non-blank character after the Q or A and
continues until the end of the line.

Each 'Q' line is followed immediately by two blocks of 'Q' and 'A'
lines. The first block describes the collection of questions and
answers relevant following a "yes" answer to the first question. The
second block describes the collection of questions and answers
relevant to a "no" answer to the opening question.

For example,

Q Does it live in the water?
Q   Does it have webbed feet?
A     Duck
A     Fish
A   Cat


Describes a tree in which the first question to be asked is "Does it
live in the water?". If the person playing the game answers "yes",
then the block of lines

Q   Does it have webbed feet?
A     Duck
A     Fish

is relevant (i.e., the program will next ask about webbed feet). If
the person answers "no". then the block of lines

A   Cat

is relevant (i.e., the program will next ask "Is it a cat?".

The "indentation" shown in the sample above is purely for human
readability.  It is not required in your output, though your input
routine should tolerate it if it is present.

How to use:
You must supply one command line argument, the name of the datafile to read and write the questions/answers.
During execution, you are able to add new questions and answers by following the prompts and answering 'no' or 'n'.

For each question, you can answer with either a 'yes' or a 'no'.
