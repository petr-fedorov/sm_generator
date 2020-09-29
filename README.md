# Enhanced State Machine Generator for BOUML

[BOUML](https://www.bouml.fr/) is a free UML 2 tool box including a modeler allowing you to specify and generate code in C++, Java, Idl, Php, Python and MySQL.

BOUML is extensible, and the external tools named plug-outs can be written in C++ or Java, using BOUML for their definition as any other program. Plug-outs
interact  with BOUML via a network socket. In particular BOUML contains built-in State Machine Generator that generates C++ classes implementing a behavioral state machine from a state machine diagram.

Unfortunately, generated behavioral state machines are not fully compliant with [OMG Unified Modelling Language](https://www.omg.org/spec/UML/) (hereafter UML) and [Precise Semantics of UML State Machines](https://www.omg.org/spec/PSSM/) (hereafter PSSM) specifications as shown in the table below. Enhanced State Machine Generators aims to improve that situation. The current status of the effort is shown in the table too.


| Test | Built-in State Machine Generator | Enhanced State Machine Generator |
|------|:-----------------:|:----:|
|UML-Compound Transition Example | :x: |  :heavy_check_mark: |
|PSSM-Entering 004 | :x:   |  :heavy_check_mark:  |
|PSSM-Entering 005 |  :x:  |  :heavy_check_mark: |
|PSSM-Entering 009 | :x:   | :heavy_check_mark:   |
|PSSM-Event 016 | :x:   |  :heavy_check_mark:  |
|PSSM-Event 018 | :heavy_check_mark:   |  :heavy_check_mark:  |
|PSSM-Exiting 001 | :x:   |  :heavy_check_mark:  |
|PSSM-Exiting 004 | :heavy_check_mark:   |  :heavy_check_mark:  |
|PSSM-Exit 001 |:heavy_check_mark:    |  :heavy_check_mark:  |
