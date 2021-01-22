# Statixtest
This is a Spoofax project that adds some conveniences to the scope graph part
of Statix test result files (`.stxresult`).
Firstly, it allows following references in the scope graph by CTRL/CMD+clicking
the reference.
Secondly, it adds menu entries Spoofax > Generate > Merge declarations into
scopes in [this|new] file.
The menu entries merge the declarations (matching regex `#-d_\d+-\d+`, e.g.
`#-d_398-38`) into the scopes where they are declared.
This makes the scope entries more concise and improves readability.

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

After the import is complete it should be loaded.
You will need to close and re-open any `.stxresult` files you have open.
In case it doesn't work immediately, try restarting eclipse (file > restart).
