# EC-based Reasoning System
Reasoning system based on Clingo.

## System
- OS:
    -- Windows 10
    -- Ubuntu
- Clingo - 5.4.0

## Folders
- [./clingo/](https://github.com/MorphSeur/OnlineECParser/tree/master/clingo) - Contrains [clingoWindows.exe]() and [clingoLinux]() and [format-output13042022_2.exe]() and [format-output13042022_4.bin]() files. And [format-output13042022.cc] source code.
- [./lp/](https://github.com/MorphSeur/OnlineECParser/tree/master/lp) - Contrains:
    -- activities.lp - affordances.  
    -- events.lp - happens.  
    -- sorts.lp - locations and objects of interests coming from low-level layer.  
    -- ecasp888.lp - events and fluents, effects of events and triggered event.  
    -- ecasp88888.lp - context predicates linking the affordances.  
    -- decOrigin2.lp - Discrete Event Calculus Axiomatization.  
    
- [./inference/](https://github.com/MorphSeur/OnlineECParser/tree/master/inference) - contains the inference in file ecasp88.txt in line 15.  

- parserEC.ipynb - is the parser.  


## Important:
If permission denied, run:  
- $ chmod +x clingoLinux  
- $ chmod +x format-output13042022_4.bin

### format-output13042022_2.exe and format-output13042022_4.bin
The answer set interpreters allow to handle 103500 predicates.  
These interpreters avoid showing the Clingo answer sets (line 89 and 90).


### format-output13042022.cc
The source code of the interpreters.  
The interpreters were compiled using [g++34](https://stackoverflow.com/questions/33452554/how-to-use-g-3-4-in-ubuntu-15-04) version 3.4.6 for linux and [i586-mingw32msvc-g++](https://stackoverflow.com/questions/2033997/how-to-compile-for-windows-on-linux-with-gcc-g) version 4.2.1 for windows.