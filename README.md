# Bash Delectable Scripting Modules (BDSM) Framework

BDSM is a system scripting DSL & framework for beating software and systems
into submission

# Goal

The goal is to create an extensible scripting framework providing a very robust
DSL. A primary tennant of BDSM is that it must handles as much pain as possible
so that users of the BDSM DSL modules can create high quality extensions and
expose their commands through BDSM's flexible command line interface (CLI).

# Architecture

BDSM itself is a scripting framework which provides very rich DSL sets known as
modules. Users of BDSM may use the DSL to write 'extensions' which are
essentially named sets of scripts (directories!). Users of BDSM may also easily
install and manage a multitude of extensions and sets of extensions providing
functionality only limited by the creative abilities of extension authors :)

# Creating Extensions

There are only a few requirements for the 'extensions'. The extension must be a
directory. Within this directory are (at least) the subdirectory bin/ with at
least one executable file called 'help'. Additionally in the root of the
extension directory there must be a text file called VERSION with a version
number that follows semantic versioning (http://semver.org/) in the format of
X.Y.Z where X,Y and Z are positive integers. An extension must also have a
README file in which you should explain about the extension.

The contents of the bin directory can be *any* execuatble file.  This means for
example that C compiled binaries, Ruby Scripts, python, lua, etc... may all be
used according to requrements and/or user preferences.  Of course the extensions
which *I* write will likely be in bash ;) Additionally if you write your
extensions in bash a nice DSL is automatically loaded for you. Read more
about the DSL in the online documentation.

  ~Wayne

Wayne E. Seguin
wayneeseguin@gmail.com
http://github.com/wayneeseguin
http://twitter.com/wayneeseguin
https://bdsm.beginrescueend.com/
https://rvm.beginrescueend.com/

# Contributing

In the spirit of free software, everyone is encouraged to help improve this project.

Here are some ways you can contribute:

by using the latest development and release versions
by reporting bugs in #beginrescueend on irc.freenode.net
by suggesting new features in #beginrescueend on irc.freenode.net
by writing or editing documentation, which is greatly appreciated
by translating documentation to a new language, I speek tech and poor engrish
by writing extensions
by writing code (no patch is too small: fix typos, add comments, clean up inconsistent whitespace)
by performing code reviews and assisting with refactoring
by resolving issues
by reviewing patches
by donating, xoxo!

# License

All BDSM Core scripts and extensions themselves are are licensed under
the Apache License v2.0

Copyright (c) 2009-2011 Wayne E. Seguin

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

License Exceptions:

bin/bdsm-ll is GNU Parallel and is licensed under the GNU GPL v3 which can be
read here: http://www.gnu.org/licenses/gpl.html

