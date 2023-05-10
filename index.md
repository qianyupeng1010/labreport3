# Lab Report 3
## `less`command
### Option 1: `less -s`
`less -s` combines successive blank lines into one blank line.<br>
**First Example:**<br>
if we put `less technical/biomed/1468-6708-3-3.txt` into the terminal, part of the output would be:<br>
```
The Myocardial Ischemia Reduction with Aggressive Cholesterol Lowering (MIRACL) trial set out to answer this question.
      
      
The answer?
MIRACL enrolled 3,086 patients within 24-96 hours (mean
63 hours) of admission for unstable angina or a non-Q-wave
myocardial infarction and randomized them to 16 weeks of
atorvastatin 80 mg or placebo once daily [ 5 ] .
```

but if we put `less -s technical/biomed/1468-6708-3-3.txt` into the terminal, this part of the output would be:<br>
```
The Myocardial Ischemia Reduction with Aggressive Cholesterol Lowering (MIRACL) trial set out to answer this question.

The answer?
MIRACL enrolled 3,086 patients within 24-96 hours (mean
63 hours) of admission for unstable angina or a non-Q-wave
myocardial infarction and randomized them to 16 weeks of
atorvastatin 80 mg or placebo once daily [ 5 ] .
```
This command is useful because if provide more space for more contents.<br>
**Second Example:**<br>
if we put `less technical/plos/journal.pbio.0020001.txt`in to the terminal, part of the output would be:<br>
```
much higher percentage than the increments reached by Europe (10%) and industrial Asia
(26%). The percentage of global scientific publications from North America actually
decreased by 8% over the same period (UNESCO 2001).


Publishing Trends in the Americas
Using the SCI databases produced by the Institute for Scientific Information (ISI), as
well as data compiled by the Red Iberoamericana de Indicadores de Ciencia y Tecnología
(RICYT), 
```

but if we put `less -s technical/plos/journal.pbio.0020001.txt`in to the terminal, this part of the output would be:<br>
```
much higher percentage than the increments reached by Europe (10%) and industrial Asia
(26%). The percentage of global scientific publications from North America actually
decreased by 8% over the same period (UNESCO 2001).

Publishing Trends in the Americas
Using the SCI databases produced by the Institute for Scientific Information (ISI), as
well as data compiled by the Red Iberoamericana de Indicadores de Ciencia y Tecnología
(RICYT), 
```
This command deleted one blank line and leave more space to display more contents.<br>
[Website Cited](https://phoenixnap.com/kb/less-command-in-linux)
### Option 2: `less -M`
When the user is reading a file using the `less`command with the `-M` option, it also enables the display of reading statistics such as the current line number and the percentage of content that has been read.<br>
**First Example:**<br>
If we put `less -M technical/plos/journal.pbio.0020001.txt` in terminal, it will show in terminal:
```
 Kofi Annan, the Secretary-General of the United Nations, recently called attention to
        the clear inequalities in science between developing and developed countries and to the
  
    
      
    
      
        
        Kofi Annan, the Secretary-General of the United Nations
, recently called attention to
        the clear inequalities in science between developing an
d developed countries and to the
        challenges of building bridges across these gaps that should bring the United Nations and
        the world scientific community closer to each other (An
nan 2003). Mr. Annan stressed the
        importance of reducing the inequalities in science betw
een developed and developing
        countries, asserting that “This unbalanced distributiontechnical/plos/journal.pbio.0020001.txt lines 6-11/231 3%
```

`less -M` provided us the information `distributiontechnical/plos/journal.pbio.0020001.txt lines 6-11/231 3%` This shows we have read 3% of the text<br>
**Second Example:**
<br>
If we put `less -M technical/911report/chapter-1.txt` into terminal, we will get

```
Washington Dulles: American 77. Hundreds of 
miles southwest of Boston, at Dulles Internation
al Airport in the Virginia suburbs of Washington
, D.C., five more men were preparing to take the
ir early morning flight. At 7:15, a pair of them
, Khalid al Mihdhar and Majed Moqed, checked in 
at the American Airlines ticket counter for Flig
ht 77, bound for Los Angeles. Within the next 20
 minutes, they would be followed by Hani Hanjour
 and two brothers, Nawaf al Hazmi and Salem 
 cal Hcal/911report/chapter-1.txt lines 37-38/731 4%
 ```
 
 Here the command `less -M` provide us the information:`cal Hcal/911report/chapter-1.txt lines 37-38/731 4%` It shows we have read 4% of the text.<br>
This command is useful because it could tell us how many percent of the content we have read.
[website Cited](https://phoenixnap.com/kb/less-command-in-linux)

### Option 3: `less -N`
`less -N` will display the line numbers at the beginning of each line.<br>
**First Example:**<br>
If we put `less -N technical/911report/chapter-2.txt` into the command, it will give us the output like this:

```
      1 
      2     
      3         
      4             THE FOUNDATION OF THE NEW TERRORISM
      5             A DECLARATION OF WAR
      6             In February 1998, the 40-year-old Saudi exile Usama Bin Ladin and a fugitive Egyptian
      7                 physician, Ayman al Zawahiri, arranged from their Afghan headquarters for an Arabic
      8                 newspaper in London to publish what they termed a fatwa issued in the name of a
      9                 "World Islamic Front." A fatwa is normally an interpretation of Islamic law by a
     10                 respected Islamic authority, but neither Bin Ladin, Zawahiri, nor the three others
     11                 who signed this statement were scholars of Islamic law. Claiming that America had
      ...
    941 minded these bombings, Bin
    942                 Ladin said that the World Islamic Front for jihad against "Jews and Crusaders" had
    943                 issued a "crystal clear" fatwa. If the instigation for jihad against the Jews and
    944                 the Americans to liberate the holy places "is considered a crime,"he said,"let
    945                 history be a witness that I am a criminal."
    946             
    947         
    948     
~
~
~
(END)
```
**Second Example:**
If we put `less -N technical/911report/chapter-3.txt` into the command, it will give us the output like this:
 ```
      1 
      2     
      3         
      4             COUNTERTERRORISM EVOLVES
      5             In chapter 2, we described the growth of a new kind of terrorism, and a new terrorist
      6                 organization-especially from 1988 to 1998, when Usama Bin Ladin declared war and
      7                 organized the bombing of two U.S. embassies. In this chapter, we trace the parallel
      8                 evolution of government efforts to counter terrorism by Islamic extremists against
      9                 the United States.
      ...
   3150                 into Afghanistan, perhaps as part of a team joined to a deployment of the CIA's own
   3151                 officers, would have required a major policy initiative (probably combined with
   3152                 efforts to secure the support of at least one or two neighboring countries) to make
   3153                 a long-term commitment, establish a durable presence on the ground, and be prepared
   3154                 to accept the associated risks and costs. Such a military plan was never developed
   3155                 for interagency consideration before 9/11. As 1999 came to a close, the CIA had a
   3156                 new strategic plan in place for capturing Bin Ladin, but no option was rated as
   3157                 having more than a 15 percent chance of achieving that objective.
   3158         
   3159     
(END)
```
This command is useful because it can help us identify which line we are reading and give us a easier reference to contents in a specific line.
[website Cited](https://phoenixnap.com/kb/less-command-in-linux)


### Option 3: `less -p[pattern]`
`less -p[pattern]` will highlight the search pattern in the output and find the first occurrence of the specified pattern in the input file.<br>
**First Example:**
If we put `less -pnational technical/911report/chapter-6.txt`, it will give us the output like this:<br>

<img width="753" alt="截屏2023-05-10 下午3 49 01" src="https://github.com/qianyupeng1010/labreport3/assets/130001791/96fd0910-eecc-44af-b29e-103334ba0990">

`less -pnational` highlighted the word `national` in the text.
**Second Example:**
If we put `less -pspotted technical/911report/chapter-7.txt`, it will give us the output like this:<br>

<img width="739" alt="截屏2023-05-10 下午3 51 07" src="https://github.com/qianyupeng1010/labreport3/assets/130001791/f4d35a7e-18f6-492c-9dbf-7367105976f7">
`less -pspotted`highlighted the word `spotted` in the text.
This command is useful because if we want to find keyword in a text, this command could do what we want.
[Website Cited](https://phoenixnap.com/kb/less-command-in-linux)






















