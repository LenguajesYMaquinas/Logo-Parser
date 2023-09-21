# Logo Parser

## About this

This program is a parser for a part of the Logo programming language, specifically between the [lesson 1](https://www.turtleacademy.com/lessons/1) and [lesson 14](https://www.turtleacademy.com/lessons/1). The production rules are in EBNF grammar are on the [production_rules](/production_rules.pdf) file.

## Technologies

- Java
- JavaCC

## Respository files

  The important files are:

- [Logo.jj](/src/lym/languages/SwiftViews.jj): this is the main file and contains the parser code.

## Considerations

- The separator betwwen comands is newline (\n).
- The sintaxys for strings is: !<STRING>.

## Execution

<ol>
<li>Create a new java project on Eclipse</li>
<li>Copy the files of this repository on the project created</li>
<li>Open the [ConsolaParsers.java](/src/lym/interfaz/ConsolaParsers.java) file and execute it</li>
<li>Write code on the bottom section of the interface and click on the *Enviar* button</li>
<li>If  the input was a valid program, the interface will return *OK*</li>
</ol>

##The following is a valid program:

forward 50
left 90
forward 50
fd 50
lt 90
fd 30
pendown
penup
cs
home
setx 100
sety 100
setxy 50 50
seth 175
arc 90 60
arc 360 100
csh "cat
repeat 24 [ rt 17
fd 33]
print heading
print towards list 0 0
seth 212.5
label !turtle
repeat 4 [ fd 100
lt 90]
repeat 5 [setwidth 1
fd 10
setwidth 3
fd 10]
repeat 5 [setwidth 1
fd 10
setwidth 3
fd 10]
lt 45 ]
to dashline repeat 5 [setwidth 1
fd 10
setwidth 3
fd 10] end
repeat 4 [rt 90
dashline]
print random 16
setcolor random 16
fd 50
make "z difference :x :y
to going :fdinput fd :fdinput end
going 150
to polygon :edges repeat :edges [fd 100
rt 360/:edges] end
for [i 1 100] [fd :i * 10 
rt :i]
to spiral :size if :size > 30 [stop] fd :size rt 15 spiral :size *1.02 end
