# Statixtest
This is a Spoofax project that adds some conveniences to the scope graph part
of Statix test result files (`.stxresult`) and scope graph files (`.scopegraph`).
Firstly, it allows following references to scopes in the scope graph by
CTRL/CMD+clicking the reference.
Secondly, it adds menu entries in `Spoofax > Format`
- `Format` executes all other formatting actions from `Spoofax > Format`
- `Remove empty elements in scopes` removes empty sets in scopes, e.g. if a
   scope doesn't have edges it will remove. `edges { }`
- `Replace HTML codes` replaces HTML codes in `.stxresult` errors, warnings and
   notes with their proper characters.

# Instructions
Using this project is easy: just load it in Spoofax and it will automagically
work.

1. Checkout this repository using git or by downloading a .zip
2. Import the project in eclipse:
   1. File > import
   2. Maven > existing maven projects
   3. Select the root directory, select `/pom.xml`
   `org.metaborg.statixtest:0.1.0-SNAPSHOT:spoofax-language` (should be the
   only option), click finish
3. Build the project (project > Build Project)

After the build is complete it should be loaded.
You will need to close and re-open any `.stxresult` files you have open.
In case it doesn't work immediately, try restarting eclipse (file > restart).
