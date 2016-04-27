# Coati Bug Tracker
Public bug tracker of Coati (http://coati.io)

Post all your feature requests and bug reports here.

## Reporting

Please report bugs in the issues section of this repository. Use the following template:

* platform version:
* Coati version:
* description of the problem:
* steps to reproduce the problem:

If you don't have a GitHub account you can also write an e-mail to support@coati.io and we will take care of it.

## Supporting

If you want to support a certain feature request or you have the same bug another user already reported, then please let us know:
* post a comment with "+1" to the issue
* or send an email to support@coati.io with the issue ID

Thank you!

## Changelog

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
