# eepAssembler

A simple assembler for EEP1 CPU as taught at Imperial College 2023

*This code is written by Tom Clarke with no guarantee as to its correctness: please e-mail me if you find errors*

Use issues on this repo for feature requests

The F# source is in `./src/Program.fs`

## To run the assembler

Before you start:

* Download and unzip the latest release source code or fork and clone this repo.
* Install [.NET SDK 6](https://dotnet.microsoft.com/en-us/download). (If you have .NET 7 SDK installed that will also work).

To run the assembler on any system (see nicer option via windows powershell below):

* start a command line terminal running in this directory (the one containing the downloaded README file).
* `dotnet run dir`
   * replace `dir` by the directory you want to watch
* `dotnet run` will watch `.`

### From Windows via powershell

Double-click `chooser.bat` from this directory to use file selection GUI - the whole directory of file selected will be watched.

## Features

* The assembler will watch a directory and turn any `.txt` file into a `.ram` file suitable for use by Issie, or print out errors.
* Files that change will get re-assembled, so you can edit a file and save it with auto-assembly on save.
* Lines can be labelled (see `assembler.txt`) and labels used in jump or memory instructions as Imm8 operands.



## To develop

On windows:
* Install *Visual Studio 2022* with F# desktop
* (if needed) install [.NET SDK](https://dotnet.microsoft.com/en-us/download/visual-studio-sdks) 
* load `./eepassem.sln`

See [HLP setup](https://intranet.ee.ic.ac.uk/t.clarke/hlp/install-notes.html) for more details of different dev environments.


