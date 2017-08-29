# Sourcetrail Bug Tracker
Public bug tracker of Sourcetrail (https://sourcetrail.com)

Post all your feature requests and bug reports here.

## Reporting

Please report bugs in the issues section of this repository. Use the following template:

* platform version:
* Sourcetrail version:
* description of the problem:
* steps to reproduce the problem:

If you don't have a GitHub account you can also write an e-mail to support@sourcetrail.com and we will take care of it.

## Supporting

If you want to support a certain feature request or you have the same bug another user already reported, then please let us know:
* post a comment with "+1" to the issue
* or send an email to support@sourcetrail.com with the issue ID

Thank you!

## Changelog

#### 2017.3.26
released 2017-08-24

* Java: fixed indexer to continue working when a dependency path does not exist
* Changed default indexer thread count to 0, which uses optimal thread count
* Java: Changed default value for maven dependencies directory
* Java: improved indexing speed to be 2.5 time faster
* Added commandline API for indexing projects and configuring indexing related preferences (issue [#383](https://github.com/CoatiSoftware/CoatiBugTracker/issues/383))
* Mention call/inheritance graphs in tutorial
* CXX: Save command line info of indexer command to errors and show within errors table (issue [#351](https://github.com/CoatiSoftware/CoatiBugTracker/issues/351))
* CXX: Added cross-compilation UI to project setup (issue [#370](https://github.com/CoatiSoftware/CoatiBugTracker/issues/370))
* Added update checker connecting to online API and checkbox to enable daily update checks on start screen.
* Java: Implemented interrupting AST visiting of Java indexer
* Java: Updated to JavaSymbolSolver 0.6.0.X and Javaparser 3.3.0
* CXX: Removed preprocessor only option, because of new include path validation
* CXX: Fixed uppercase CXX header file name and extensions saved in lowercase (issue [#437](https://github.com/CoatiSoftware/CoatiBugTracker/issues/396))
* Code: When clicking source location with multiple tokens or local symbols show a list to select one of these
* Sort indexer commands for increased performance
* Added custom tooltipping to Code and Graph with clickable types of variables and signatures (issue [#195](https://github.com/CoatiSoftware/CoatiBugTracker/issues/195), [#331](https://github.com/CoatiSoftware/CoatiBugTracker/issues/331))
* Java: fix issue where Maven project did not show any source files (issue [#428](https://github.com/CoatiSoftware/CoatiBugTracker/issues/428))
* CXX: clean indexed header path selection for project setup from Compilation Database
* Added progress dialog for "show source files" button in project setup UI
* CXX: Added include path validation to project settings
* Search: Select text elements when clicking into search bar
* Search: Fixed crash when fulltext search yields no results
* Updated to Qt 5.9.1
* CXX: Added node type for "union"
* CXX: Merge anonymous types and the respective typedef (issue [#189](https://github.com/CoatiSoftware/CoatiBugTracker/issues/189), [#292](https://github.com/CoatiSoftware/CoatiBugTracker/issues/292))
* CXX: Updated to clang 4.0.1
* Added Menu option to show Start Window
* Don't show start window when opening project with double-click
* Show license type label in title bar: "Sourcetrail [trial, test, non-commercial]"
* Graph: Fixed class expand toggle shown in overview and namespace lists
* Graph: Show inheritance edges between parents of active symbol and other visible symbols (issue [#167](https://github.com/CoatiSoftware/CoatiBugTracker/issues/167))
* Improved project loading performance
* Code: improved location retrieval and hover performance
* Show recent bookmarks in bookmarks menu (issue [#414](https://github.com/CoatiSoftware/CoatiBugTracker/issues/414))
* Code: Fixed references and buttons when activating file in snippet mode
* Java: added auto-detection for JRE System Library
* Java: Prefill JRE system library path on first Sourcetrail launch
* macOS: fixed qt.conf for case-sensitive file system (issue [#404](https://github.com/CoatiSoftware/CoatiBugTracker/issues/404))
* Improved database saving performance
* Improved database file clearing performance
* Improved contrasts of UI elements in bright color scheme
* Graph: Show zoom level as percent label next to zoom buttons
* Added Visual Studio Code plugin (issue [#397](https://github.com/CoatiSoftware/CoatiBugTracker/issues/397))
* Added "Edit Project" button below error table
* Java: Maven fixes regarding JAVA_HOME variable (issue [#405](https://github.com/CoatiSoftware/CoatiBugTracker/issues/405))

#### 2017.2
released 2017-06-21

* Fixed crash when using shortcuts containing letters with focus on the graph on macOS (issue [#390](https://github.com/CoatiSoftware/CoatiBugTracker/issues/390))
* Improved Visual Studio plugin performance
* Updated End User License Agreement and have users accept on first run on macOS and Linux
* Fixed memory issues when using large Compilation Database files (issue [#396](https://github.com/CoatiSoftware/CoatiBugTracker/issues/396))
* Updated to JavaParser and JavaSymbolSolver
* Fixed issue where black borders appeared around dialogs for some Linux window managers (issue [#376](https://github.com/CoatiSoftware/CoatiBugTracker/issues/376))
* Use platform default window decorations for UI dialogs
* Code: Made snippet minimize/maximize buttons more interactive by showing hover states
* Code: improved code view loading performance
* Java: Record more "import not found" errors
* Support Visual Studio 2017 in Visual Studio Plugin (issue [#381](https://github.com/CoatiSoftware/CoatiBugTracker/issues/381))
* Graph: increased creation speed by requesting less data
* macOS: Codesign .app bundle to avoid "from unidentified developer" warning
* Error: Use same error order in error table and code view
* Error: Only show first 1000 errors, click button in lower right of error table to show all (issue [#385](https://github.com/CoatiSoftware/CoatiBugTracker/issues/385))
* Graph: use bezier edges when activating aggregation edge
* Send ping after changing plugin ports
* Added menu action to display EULA and force accepting on macOS
* Fixed use of environment variables in project setup paths
* Multi-language project setup via Source Groups setup UI (issue [#230](https://github.com/CoatiSoftware/CoatiBugTracker/issues/230))
* C/C++: Fixed no files indexed when relative file paths are provided in Compilation Database (issue #388)
* C/C++: Display an error when loading a Compilation Database fails
* C/C++: Fixed source files within Compilation Database not indexed unless within Indexed Header Paths
* Fixed status message length limiting window resizing (issue [#372](https://github.com/CoatiSoftware/CoatiBugTracker/issues/372))
* Match source file extensions case insensitive (issue [#384](https://github.com/CoatiSoftware/CoatiBugTracker/issues/384))
* Fixed indexing progress file count in status bar and status view (issue [#387](https://github.com/CoatiSoftware/CoatiBugTracker/issues/387))
* Windows: remove setup.exe from windows installer with all necessary .dll files
* Added history list button between back and forward button
* Added history menu showing activated symbols in chronologic order

#### 0.12.25
released 2017-05-16

* Added QtCreator plugin
* Graph: Added context menu action to create bookmark for node under mouse cursor (issue [#373](https://github.com/CoatiSoftware/CoatiBugTracker/issues/373))
* Code: Fixed code view not scrolled to first fulltext search match in single file mode
* Set unrestricted permission for accessing shared memory to fix crash on Windows
* Improved setting descriptions in preferences dialog
* Java: Updated to JavaParser 3.2.0 and JavaSymbolSolver 0.5.3
* Graph: Fixed order of nodes is same as within first encountered header file
* Save timestamp after project indexing and show it on the overview screen
* Fixed use of correct name delimiters in indexer processes
* Fixed crash when running 32 and 64 bit versions in parallel
* Bookmark: Changed menu action to "Bookmark Active Symbol"
* Graph: Zooming on Ctrl + Mouse Wheel now (Shift + Mouse Wheel still working)
* Added dialog to warn about "verbose indexer logging" before indexing.
* Added multi process indexing for C/C++ projects to better handle crashes during indexing.
* Reduced file accesses during C/C++ indexing.
* Graph: Show call graphs, inheritance trees and include trees for active symbol. UI in the top left of the graph view for defining direction and depth. (issues [#249](https://github.com/CoatiSoftware/CoatiBugTracker/issues/249) [#337](https://github.com/CoatiSoftware/CoatiBugTracker/issues/337))
* Improved performance by running UI updates in parallel for each view
* Fixed project refresh not recognizing newly added files
* Show progress dialog when clicking refresh while computing files (issue [#341](https://github.com/CoatiSoftware/CoatiBugTracker/issues/341))
* Added show files button to summary of compilation database project setup (issue [#354](https://github.com/CoatiSoftware/CoatiBugTracker/issues/354))
* Show option to run only C/C++ preprocessor when indexing on indexing start dialog (issue [#297](https://github.com/CoatiSoftware/CoatiBugTracker/issues/297))
* Added bookmarking feature for nodes and edges. Bookmarks can have categories and comments. Data gets stored in .srctrlbm next to project file. Shortcuts similar to web browsers. (issue [#138](https://github.com/CoatiSoftware/CoatiBugTracker/issues/138))
* Mark files with errors and all files within a translation unit with fatal errors as incomplete (issue [#358](https://github.com/CoatiSoftware/CoatiBugTracker/issues/358))
* Fixed compilation database projects using C++ source extensions and standard (issue [#366](https://github.com/CoatiSoftware/CoatiBugTracker/issues/366))

#### 0.11.86
released 2017-04-12

* Terminating all running tasks before closing the application (issue [#343](https://github.com/CoatiSoftware/CoatiBugTracker/issues/343))
* Use all available cores when setting indexer threads to 0 (issue [#342](https://github.com/CoatiSoftware/CoatiBugTracker/issues/342))
* Added reset window layout option to view menu (issue [#289](https://github.com/CoatiSoftware/CoatiBugTracker/issues/289))
* Fixed colorscheme gets refreshed when cancelling preferences dialog
* Log: Scroll to first line in errors table after indexing and after display
* Copy old ApplicationSettings.xml and window_settings.ini files from previous Coati install if available.
* New projects are created with .srctrlprj and .srctrldb endings, but still support old file extensions.
* Renamed application from Coati to Sourcetrail
* Fixed issues in tutorial project
* Graph: Fixed node with no children but qualifier shows expand button
* Enable undo/redo actions in context menu only when available
* Java: Updated to JavaParser 3.1.2 and JavaSymbolSolver 0.5.2.x
* Revised undo/redo stack to handle messages differently
* Java: Added support for project setup from Maven
* Windows: Hide console when running release builds
* Show license information on start screen
* Added ping support to plugins and display current connected editor/IDE in status bar.

#### 0.11.15
released 2017-03-01

* Don't accept richt text in 'enter license' dialog field (issue [#207](https://github.com/CoatiSoftware/CoatiBugTracker/issues/207))
* Updated EULA to include Test License and better clarify other license types
* Fixed icons in project setup dialogs blurry on highDPI screens
* Added link to additional downloadable pre-indexed projects to trial start screen
* Fixed crash when saving preferences if they contain relative paths
* Convert all paths chosen by patch picker relative to project location in project setup
* Disabled name and location changing in project editing and removed project moving
* Split default file extensions for C++ and C to avoid wrong files getting indexed
* Deprecated 'Lazy Include Search', it's only visible to previously created projects (issue [#335](https://github.com/CoatiSoftware/CoatiBugTracker/issues/335))
* Support relative paths and paths containing environment variables for compilation database path (issue [#312](https://github.com/CoatiSoftware/CoatiBugTracker/issues/312))
* Removed 'Advanced Settings' section in project setup and show theses options in separate dialog (issue [#293](https://github.com/CoatiSoftware/CoatiBugTracker/issues/293))
* Support environment variables containing multiple files in project setup paths (issue [#283](https://github.com/CoatiSoftware/CoatiBugTracker/issues/283))
* Warn users when no 'Indexed Header Paths' were set in compilation database project (issue [#254](https://github.com/CoatiSoftware/CoatiBugTracker/issues/254))
* Renamed "Project Paths" to "Indexed Paths" in project setup
* Renamed "Project File Location" to "Coati Project Location" in project setup (issue [#234](https://github.com/CoatiSoftware/CoatiBugTracker/issues/234))
* Allow opening indexed projects in trial mode
* Record node type of non-indexed qualifiers (e.g. "std" in "std::string" as namespace)
* Log: Fixed error icon loaded for every row (issue [#287](https://github.com/CoatiSoftware/CoatiBugTracker/issues/287))
* Graph: Fixed lambda are placed within white area to better see call edges
* Graph: Show non-indexed nodes within their parents instead of using namespace labeling
* Code: Disabled syntax highlighting for project description
* Graph: Fixed different font-faces causing graph nodes to expand to bigger cell amount
* Mac: Fixed wrong READMEs at some plugins (issue [#315](https://github.com/CoatiSoftware/CoatiBugTracker/issues/315))
* Mac: Removed boost libraries and libLTO from Mac bundle
* Windows: Add Visual Studio compatibility flags to new project when Visual Studio include paths are present
* Renamed undefined nodes to non-indexed nodes for clarification
* Show progress in file clearing dialog
* Extended syntax highlighting for Java and distinguish by project type
* offer Windows 64bit build (issue [#300](https://github.com/CoatiSoftware/CoatiBugTracker/issues/300))
* Fixed legacy Java 6 install necessary on MacOS (issue [#280](https://github.com/CoatiSoftware/CoatiBugTracker/issues/280))
* Updated to Qt 5.8
* Updated to clang/llvm 3.9
* Added multithreading to Visual Studio plugin compilation database creation
* Graph: Use new list layouting for overview bundles and namespaces/packages
* Graph: Group nodes in list layout by starting character and allow jumping to group by pressing the key
* Graph: Use node specific styles for overview bundles
* Visual Studio plugin can now handle projects with non-native build tool for compilation database export
* Changed menu action 'Licenses' to '3rd Party Licenses'
* Added dialog with all shortcuts to Help menu
* Log: Show error in errors table when clicked in code view (issue [#323](https://github.com/CoatiSoftware/CoatiBugTracker/issues/323))
* Code: Switched default mouse drag behavior to selection, panning on Shift + drag, and show suitable cursors
* Updated company address in about dialog
* Graph: Added on-screen zoom buttons
* Graph: Split aggregation edge when expanding nodes if possible
* Uncommented lines using the std library in TicTacToe sample
* Fixed issue with lambda return type (issue [#318](https://github.com/CoatiSoftware/CoatiBugTracker/issues/318))
* Save builtin types as separate node type (issue [#2](https://github.com/CoatiSoftware/CoatiBugTracker/issues/2))
* Remove unused included files after refreshing
* Java: Fixed packages that only contain packages to show up as non-indexed
* Added context-menu actions to copy node names, file paths and show files in containing directory (issue [#320](https://github.com/CoatiSoftware/CoatiBugTracker/issues/320))
* Fixed crash when entering a single space in 'enter license' dialog (issue [#277](https://github.com/CoatiSoftware/CoatiBugTracker/issues/277))
* Graph: Made edge lines thicker
* Fixed handling and storing of files with the same name
* Fixed environment variable detection within project paths for %VARIABLE_NAME% syntax
* Coati states whether it needs 32bit or 64bit JRE
* Java: Updated indexer to fix a lot of unsolved symbol issues
* Graph: Fixed layouter couldn't handle nodes with same name
* Graph: Fixed weird looking vertical aggregation edges to child nodes
* Code: Don't show stats for non loaded project
* Added option to disable UI animations to preferences
* Graph: Removed double line around graph view on Mac
* Graph: Fixed namespace label cut off at edge of screen
* Code: Added single file view mode
* Code: Added navigation bar with mode toggle and buttons to navigate references
* Graph: Removed underscores in edge hover names
* Infere some non-indexed node types by their edges


#### 0.10.0
released 2016-12-14

* Windows: Added runtime DLLs that could be missing on some systems
* Click message in status bar to open status window
* Graph: Sort nodes alphabetically within each section
* Graph: Aggregate type use edges to make referencing nodes appear collapsed
* Code: Improved performance through faster source location retrieval for files
* Code: Scroll active symbol definition to top of view if possible
* Added status tab to Log View showing status bar information
* Graph: Fixed graph animation used when clicking edges
* Graph: Disable bundling when files or macros are active
* Graph: Bundle importing files of active symbol in Java projects
* Improved speed of depending file search on refresh
* Search: Fixed crashes related to empty searches (issue [#251](https://github.com/CoatiSoftware/CoatiBugTracker/issues/251))
* Search: Do fulltext search when no autocompletion match is available
* Added checkbox for full project refresh to start indexing dialog
* Disabled clang error limit by default to make sure all errors are shown
* Linux: Updated libs and added missing ones (issue [#245](https://github.com/CoatiSoftware/CoatiBugTracker/issues/245))
* Updated icons for some graph nodes and project types
* Windows: Updated Visual Studio plugin UI
* Graph: Fixed view to not recenter on active node when clicking edge
* Fixed wrong errors displayed, wrong error counts and error view being wrongly shown
* Removed font zoom on CTRL + MouseWheel
* Graph: Display namespace information on left side of nodes, activate namespace by clicking label
* Improved file clearing performance
* Windows: Changed setup folder layout
* Added info screen for indexer crash investigation
* Code: Fixed display of links to missing symbols in project description
* Code: Fixed snippet size calculation causing a slowdown in certain cases
* Search: Skip intermediate autocompletions when typing fast
* Show dialog for last files inserted into .coatidb at end of indexing
* Integrated Visual Studio Plugin with Coati Project creation and removed previous Visual Studio Solution parser
* Improved C++ indexer coverage: using decls, using directives, auto keyword, lambda signatures, symbol references inside lambda captures, template argument related elements
* Reduced size of .coatidb file by up to 50% for large projects
* Fixed anonymouse symbol name conflicts (issue [#241](https://github.com/CoatiSoftware/CoatiBugTracker/issues/241))
* Preferences: Added Indexer Logging option to print AST information during indexing
* Search: Added second line to search autocompletion list showing namespace, package or filepath
* Made cells readonly in errors table to prevent editing (issue [#236](https://github.com/CoatiSoftware/CoatiBugTracker/issues/236))
* Renamed Log Window to Status window


#### 0.9.23
released 2016-10-27

* Windows: Added logging and exception handling to VS plugin
* Windows: Added VC++ runtime dlls for windows installer
* Windows: Added missing VC++ runtime dlls (issue [#231](https://github.com/CoatiSoftware/CoatiBugTracker/issues/231))
* Added setting for default graph zoom on mouse wheel to preferences (issue [#237](https://github.com/CoatiSoftware/CoatiBugTracker/issues/237))
* Scroll errors table to newest error during indexing
* Fixed best scoring for search autocompletions skipped some combinations
* Fixed flickering of errors table when indexing
* Don't show error snippets in overview screen anymore
* Fixed crash when Project Paths contain files and lazy include search in enabled (issue [#201](https://github.com/CoatiSoftware/CoatiBugTracker/issues/201))
* Fixed edge cases that caused deadlocks in indexing
* Added language specific project icons to start screen
* Fixed application couldn't be quit when start screen was showing (issue [#227](https://github.com/CoatiSoftware/CoatiBugTracker/issues/227))
* Graph: Fixed missing image file ending when exporting graph for Linux
* Log Coati version when logging gets enabled
* Fixed non-indexed errors filter in errors table


#### 0.9.0
released 2016-10-14

* Extended Visual Studio Plugin to export clang Compilation Databases
* Implemented new installer for Windows
* Run System Header Include Paths and Java Path detection when starting application
* Added Log Window with Errors tab showing a table of all errors
* Added filters to bottom of error table to define which errors are displayed
* Removed ring logging and use one log file again instead
* Smaller indexing progress dialog with bar in the middle instead of golden ratio
* Code: Set default code snippet expand range to 3 lines for more context
* Graph: Fixed undoing of aggregation edge activation caused crash
* Graph: Move aggregation and inheritance edges to front when hovered or active
* Graph: Push parent nodes of active nodes to back to make all incoming and outgoing edges visible
* Properly quit application when window is closed while confirm box is open
* Properly quit application when window is closed while indexing (issue [#121](https://github.com/CoatiSoftware/CoatiBugTracker/issues/121))
* Graph: Count only top level nodes in bundle nodes of graph
* Search: Improved scoring of autocompletion matches to use best score for match
* App will go into trial mode without valid license
* Java: Auto detect java root source directories
* Fixed refresh crash (issue [#220](https://github.com/CoatiSoftware/CoatiBugTracker/issues/220))
* Java: improved indexer reliability a lot
* Java: Changed name of generic type to use name of declaration
* Fixed project refresh does not recognize removed source paths
* Java: Define maximum allocated jvm memory in preferences
* Follow symbolic directory links within source paths (issue [#205](https://github.com/CoatiSoftware/CoatiBugTracker/issues/205))
* Use white size grip in blue dialogs
* Graph: Use type node colors for undefined nodes
* Java: Show import not found as error
* Code: Select and copy source code in code view with SHIFT + mouse drag (issue [#7](https://github.com/CoatiSoftware/CoatiBugTracker/issues/7))
* Code: Added markers next to line numbers in code view showing active locations and scopes
* Merged app and trial to one build

#### 0.8.21
released 2016-09-16

* Added options for checking multiple paths in Indexed Header Paths dialog during project setup from Compilation Database [#190](https://github.com/CoatiSoftware/CoatiBugTracker/issues/190)
* Added all C/C++ standards supported by clang
* Fixed C language setting in empty project setup not propagated to indexer [#177](https://github.com/CoatiSoftware/CoatiBugTracker/issues/177)
* Added Sublime plugin to Sublime Text Package Control
* Improved indexer parallelization for faster indexing
* Changed all font-sizes to px for similar look on all platforms
* Added font face dropdown to Preferences showing all available monospace fonts [#172](https://github.com/CoatiSoftware/CoatiBugTracker/issues/172)
* Smoother font rendering on Windows by setting font engine to FreeType via qt.conf file [#137](https://github.com/CoatiSoftware/CoatiBugTracker/issues/137)
* Interrupt indexing while AST visiting for C/C++ for shorter waiting time
* Save graph as PNG image via context menu in graph view [#180](https://github.com/CoatiSoftware/CoatiBugTracker/issues/180)
* Added base folder to Linux package [#181](https://github.com/CoatiSoftware/CoatiBugTracker/issues/181)
* Use inverted golden ratio in indexing progress dialog

#### 0.8.0
released 2016-09-01

* Improved titles and help texts in project setup UI
* Fixed error locations not saved with absolute file paths in Compilation Database projects
* Added missing source files extensions setting to the Edit Project dialog [#132](https://github.com/CoatiSoftware/CoatiBugTracker/issues/132)
* Changed default text colors to black in project setup UI [#140](https://github.com/CoatiSoftware/CoatiBugTracker/issues/140)
* Added plugin ports settings to Preferences [#145](https://github.com/CoatiSoftware/CoatiBugTracker/issues/145)
* Improved project state handling on refreshing
* Added Java sample project JavaParser: http://javaparser.org/
* Fixed regex for system includes used wrongly in syntax highlighter
* Added setting to disable file and console logging, default is off [#157](https://github.com/CoatiSoftware/CoatiBugTracker/issues/157)
* Added migrations between different ApplicationSettings versions
* Added auto detection for Java library to Preferences
* Removed auto refresh option from Search view
* Added progress dialogs for indexing and block UI [#143](https://github.com/CoatiSoftware/CoatiBugTracker/issues/143)
* Hide name qualifiers for graph nodes in Java projects
* Added handling when java library not found
* Added plain text editing dialog to path list boxes
* Use language dependent symbol name delimiter in UI
* Added scroll speed setting to preferences [#112](https://github.com/CoatiSoftware/CoatiBugTracker/issues/112)
* Added Java project setup UI
* Record start and end locations of scopes in Java
* Display unresolved types names in Java as 'unresolved-type'
* Cache stats for overview to speed up display
* Fixed graph nodes to restore their expand state when going back [#118](https://github.com/CoatiSoftware/CoatiBugTracker/issues/118)
* Added shortcuts for navigating to next and previous reference in code view
* Pressing Tab in search completes up to next ::, Delete erases to last :: [#133](https://github.com/CoatiSoftware/CoatiBugTracker/issues/133)
* Bundle anonymous namespaces separately in graph overview [#126](https://github.com/CoatiSoftware/CoatiBugTracker/issues/126)
* Added 'Show Data Folder' and 'Show Log Folder' items to Help menu
* Added new status bar loader gif with higher resolution
* Record type aliases in C++
* Added Java indexer
* Changed public icon in graph and added default icon
* Scroll to file location when finding no symbol at specified location from plugin message
* Added shortcut for Preferences on Windows/Linux
* Leave code view at original line when expanding scopes
* Pan graph view to center on name of active symbol after activation
* Moved color scheme selection to Preferences
* Moved Preferences menu item to Edit menu on Windows/Linux [#113](https://github.com/CoatiSoftware/CoatiBugTracker/issues/113)
* Added setting for hiding non-fatal errors in unindexed files to preferences, turned on by default
* Fixed file out-of-date asterisk disappearing when showing snippets after minimize state
* Implemented Atom plugin: https://github.com/CoatiSoftware/atom-coati
* Implemented CLion/IntelliJ plugin: https://github.com/CoatiSoftware/idea-coati
* Implemented Eclipse plugin: https://github.com/CoatiSoftware/eCoati
* Implemented emacs plugin: https://github.com/CoatiSoftware/emacs-coati
* Improved code view rendering times
* Don't show implicit nodes in search auto completion list

#### 0.7.0.22
released 2016-07-07

* Fixed detected global header search paths lost correct order and caused problems with #include_next directives
* Fixed MaxOSX build crashed on launch due to unknown command line option passed
* Removed 'Save Project' and 'Save Project As' actions from menu
* Fixed indexer getting stuck at 'building caches' when indexing is interrupted
* Fixed database not properly closed when errors appeared during indexing
* Fixed autocompletions popup flickering while typing
* Added resize grip to bottom right corner of every dialog window
* Fixed 'paths don't exist' dialog window getting too big with lots of paths shown
* Added context menu with 'back' and 'forward' actions available in all views
* Removed Clang compiler warnings from console output
* Added handling of project specific VS macros to VS solution parser

#### 0.7.0.0
released 2016-06-15

* Updated to clang 3.8
* Fixed crash in search autocompletion retrieval due to edge case in sorting
* Fixed size policies in code view to avoid global scrollbar
* Added full text search via search field: ?<query> for case-insensitive search, ??<query> for case-sensitive search
* Made initialization for full text search lazy: done on first full text search
* Defined full text search color in all color schemes
* Increased code view performance by caching file IDs and paths
* Added multithreaded indexing. Number of threads can be set in the Preferences UI, default is 4
* Reworked graph node bundling to only distinguish defined and undefined nodes in each bucket
* Made graph node sorting alphabetical and put bundles at end
* Changed code view snippet sorting to always show definition on top
* Fixed local symbols were not available within lambdas
* Added settings for font family, font size and tab with to Preferences UI
* Fixed VS solution parser issue with internal macros
* Removed header extensions, all included files within the project paths are now analyzed
* Fixed crash in sqlite when symbol name has special characters
* Improved code view performance by reducing amount of initially open code files
* Improved graph view performance through faster data retrieval and smarter structures
* Increased aggregation click speed with faster edge id retrieval
* Fixed png color profiles to avoid console warning: "libpng warning: iCCP: known incorrect sRGB profile"
* Fixed graph edge drawn wrong when leaving from child node of smaller node
* Fixed Sublime Text Plugin issue with wrong encoding
* Randomized source file order for multithreaded analysis to increase performance
* Show name of removed symbol when going back after refreshing
* Fixed macro definition not connected to file
* Fixed macro use not found in #ifdef, #ifndef, defined() and some expand cases
* Removed back and forward steps for some graph and code view manipulations
* Fixed code view style broken on Mac due to change of working directory when analyzing compilation database
* Added database optimization step after indexing to reduce database size by ~25%
* Fixed artifacts after graph view change by clearing view
* Fixed autocompletion list highlights at wrong location for long names
* Allow files and directories to be excluded from analysis in advanced settings for project setup
* Added Qt gif plugin to Mac Release so that loader gif in status bar is visible
* Added link to download page to start screen to remind users of updating once in a while
* Check if compilation database still exists before refreshing
* Added separate step for defining project name, project location and compiliation database to project setup
* Explain that the project stays up-to-date with the compilation databes on refresh in project setup UI
* Disregard source extensions when loading from compilation database
* Removed error logs in name resolver
* Added plugin for VIM: https://github.com/CoatiSoftware/vim-coati

#### 0.6.0.0
released 2016-04-27

* Added suppport for temporary test licenses and show error message when it expired
* Increased search autocompletion performance to stay mostly below 100ms
* Increased project load performance
* Improved file clearing performance on project refresh
* Increased graph creation performance for overview screen
* Increased graph performance by reducing to fixed number of requests
* Increased graph edge drawing performance
* Improved error display performance by not expanding all of them at once
* Added analysis for local symbols and allow selecting them in the code view
* Added support for function pointers to analysis
* Smoother graph panning and zooming on keyboard using update loop
* Changed style of aggregation edge to cleaner look
* Allow certain edge types to enter and leave at top and bottom of nodes as well e.g. inheritance
* Changed namespace activation to show the namespace name in the search bar and the namespace definitions in the code view
* Differentiate between explicit and implicit nodes and only show implicit nodes in the graph view when connected
* Show deleted projects on the start screen and show messagebox to delete them
* Show analysis duration in hh:mm:ss
* Added bug tracker to the help menu
* Added home button next to search field for showing the project overview
* Added shortcut and menu item to show project overview
* Allow support for environment variables in project setup with syntax ${VARIABLE_NAME}
* Added welcome message to Coati trial
* Show quit button on license enter screen when no valid license was entered yet
* Allow color schemes to define text colors for code view highlights
* Defined new highlight colors for code view in all color schemes
* Changed style of out-of-date files to be followed by *
* Fixed Path boxes not sized correctly when switching back and forth in the project wizard
* Check analyzed paths for existence in project wizard
* Inform the user about project changes and ask before reparsing the project
* Removed "simple setup" step in project wizard and added "lazy include search"-checkbox
* Edit the project settings by clicking the project name in the overview stats
* Updated to Qt 5.6
* Improved high DPI support for windows
* Added Windows system dlls to installer on Windows so users don't not need to install the redistributable package
* Added vs-clang compatibility mode as compile flags when creating project from Visual Studio solution
* Added auto detection for system header paths to project wizard and preferences when using gcc, clang or vs compilers

#### 0.5.1.21
released 2016-03-16

* Fixed file logger using wrong directory for first log file
* Fixed crash when accessing files without read permission
* Center windows on top of main window
* Added font size limits
* Prevent network message handling without valid license
* Fixed type references in headers saved multiple times
* Improved context detection for template parameters
* Fixed Visual Studio plugin project loading
* Added delay for changing fontsize via mouse wheel
* Disabled config file warnings
* Fixed interrupting of analysis to show message in status bar
* Fixed children on namespace activation were bundled
* Fixed expanding file with errors showed all locations in red
* Show loader animation when loading project
* Removed high traffic log messages
* Fixed crash when opening newer project with older version of Coati
* Fixed project paths are now saved relative if defined relative
* Fixed project setup window sizes to adapt to content size
* Fixed linux package creating ~/.config if not there
* Show fatal errors in UI that stopped analysis
* Added compiler flags UI to advanced settings in project setup summary
* Added file extension UI to advanced settings in project setup summary
* Added graph zooming with Shift + mouse wheel or Shift + WS
* Added graph panning with WASD
* Improved project load and code view performance
* Improved analysis performance for large projects (10x as fast for 1.000.000 LoC)
* Added project setup for Compilation Databases

#### 0.5.0.4
released 2016-02-25

* Fixed preferences not saved
* Added link to documentation to Help menu
* Improved painting of icons in graph to be smoother
* Improved logging to alternate between 2 files of 1000 lines to decrease logfile sizes
* Improved analysis performance to take only 66% of the time
* Save user data in ~/Library/Application Support/Coati on Mac
* Improved style of ui windows
* Added Visual Studio solution parsing via project wizard or VS plugin
* Added project setup wizard for step-by-step project setup
* Added overview and error keywords to search view
* Show overview on project open with node bundles per type
* Added application move protection to reenter license key
* Improved log file names to be sorted chronologically
* Improved graph view node bundeling to bundle more
* Display scope name at bottom of code snippet
* Added .coatiproject file associations with icon for Mac and Windows
* Return to last scroll position when going back in code view
* Improved back & forward in code view
* Update error count while analysis
* Improved code view annotation painting performance
* Added web documentation
* Added trial target without analysis
* Added license key window and license checker
* Refresh project editing settings
* Added C and C++ standard setting to project
* Fixed cursor changing for resize and text interactions
* Added commandline option for project file
* Improved performance of token name saving
* Fixed number postions in graph
* Added shortcuts for font size resetting to View menu
* Added C support
* Added option to hide widget window title bars to View menu

#### 0.4.0
released 2016-01-07

* navigate back via backspace key
* navigate back&forward via mouse buttons
* renamed undo&redo to back&forward
* Fixed tooltip colors in dark color scheme
* Fixed style of function or method nodes with children
* Improved lambda handling in analysis
* Added help texts to project setup and preferences window
* Removed 'close window' action from menu
* Fixed constructors and destructors using return type 'void' withou source location
* Parse errors will be displayed as they appear during analysis
* Redesigned the about window
* Installing prerequisits in Windows Installer
* Added installer for Windows
* Introduced file endings .coatiproject and .coatidb for Coati's project files
* Removed Coati directory from Linux package
* Fixed graph font size was too small for Windows and Linux
* Show function and method signature in tooltip when hovering the graph node
* Added analysis for template parameter packs
* Fixed syntax highlighting to correctly identify strings, comments and block comments
* Fixed source locations of many declarations
* Coati shows a template's general definition when an implicit specialization is activated
* Added new color scheme called "bad_rainbow"
* Extended color schemes to allow more extensive use in the graph
* Coati now handles anonymous symbols when parsing files
* Improved handling of template arguments in analysis
* Coati can now handle inclass initialization of members
* Network ports for IDE communication can be defined in the ApplicationSettings.xml

#### 0.3.0
released 2015-12-14

* Saving all template arguments type uses
* Added recent projects menu option
* Focus all overlapping source locations in the code view
* Improved code view auto scroll to center the first active line in the middle
* Fixed search query disappeared when not token was found for it
* Fixed cursor was jumping at end of query when editing a search query
* Reworked code view highlighting
* Save comment locations and display them when right next to active symbol
* Fixed old data was still in new project window when creating another project
* Save macro scopes
* Save errors to storage and reactivate them via button in the status bar
* Fixed horizontal scroll in code view not activated while scrolling vertically
* Improved source locations of template scopes
* Save Coati version to sqlite and reparse project whenever the version changes
* Increased autocompletion performance by caching and limiting results to 100
* Added plugin for Sublime Text (2 & 3)
* Added plugin for Visual Studio (2012, 2013, 2015)
* Added communication interface from and to Coati via TCP sockets
* Added Tutorial project
