# Lab Report 3
## `less`command
### Option 1: `less -s`
`less -s` combines successive blank lines into one blank line.
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

but if we put 'less -s technical/biomed/1468-6708-3-3.txt` into the terminal, this part of the output would be:<br>
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
if we put 'less technical/plos/journal.pbio.0020001.txt`in to the terminal, part of the output would be:<br>
```
much higher percentage than the increments reached by Europe (10%) and industrial Asia
(26%). The percentage of global scientific publications from North America actually
decreased by 8% over the same period (UNESCO 2001).


Publishing Trends in the Americas
Using the SCI databases produced by the Institute for Scientific Information (ISI), as
well as data compiled by the Red Iberoamericana de Indicadores de Ciencia y Tecnología
(RICYT), 
```

but if we put 'less -s technical/plos/journal.pbio.0020001.txt`in to the terminal, this part of the output would be:<br>
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

### Option 2: `less -M`
When the user is reading a file using the "less" command with the "-M" option, the "-M" option instructs the "less" program to display more verbose and detailed prompts than the default "more" program. Additionally, it also enables the display of reading statistics such as the current line number and the percentage of content that has been read.
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
If we put `less -M technical/911report/chapter-1.txt' into terminal, we will get

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
 
 Here the command 'less -M' provide us the information:`cal Hcal/911report/chapter-1.txt lines 37-38/731 4%` It shows we have read 4% of the text.<br>
This command is useful because it could tell us how many percent of the content we have read.
 
 























