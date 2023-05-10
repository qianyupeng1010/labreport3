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























