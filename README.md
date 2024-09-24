# My resume

A customised fork of [Awesome-CV](https://github.com/posquit0/Awesome-CV)

Inspired by my senior's resumes: [donjar](https://github.com/donjar/Awesome-CV) and [indocomsoft](https://github.com/indocomsoft/Awesome-CV/)

## Installation

On WSL2 ubuntu:

`sudo apt install texlive-xetex texlive-fonts-extra`

This will take some minutes to download and install cos the packages are big. `texlive-xetex` gives the `xelatex` command needed for compiling the pdf, `texlive-fonts-extra` gives font-awesome and source sans pro fonts that I need. I'm sure it's possible to install in a minimal way but not worth the time exploring.

## Compilation
`make resume.pdf`

This error messages will be printed, prompting for commands. Just press enter twice and the resume.pdf will be generated. I had tried looking into it, but decided it still works anyway so I just leave it at that.

```
! LaTeX Error: There's no line here to end.

See the LaTeX manual or LaTeX Companion for explanation.
Type  H <return>  for immediate help.
 ...                                              
                                                  
l.85 
     
? 

! LaTeX Error: There's no line here to end.

See the LaTeX manual or LaTeX Companion for explanation.
Type  H <return>  for immediate help.
 ...                                              
                                                  
l.85 
     
? 

Overfull \hbox (1.46pt too wide) in paragraph at lines 85--85
[]$[]$ $[]$$[]$ 
(./resume/education.tex) (./resume/skills.tex
Overfull \hbox (24.8379pt too wide) in alignment at lines 10--28
[] [] 
) (./resume/experience.tex) (./resume/projects.tex)
(./resume/extracurricular.tex) (./resume/awards.tex) [1] (./resume.aux) )
Output written on resume.pdf (1 page).
Transcript written on resume.log.
Makefile:8: recipe for target 'resume.pdf' failed
make: *** [resume.pdf] Error 1
```

For unknown reason, the generated resume.pdf has the config to open bookmarks sidebar when opened with adobe acrobat. This can be updated using adobe acrobat. Open the file, go to File > Properties > Initial View, set Navigation tab to Page Only, then save.