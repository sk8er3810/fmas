# fmas
File Management Automation System

This is a tool to help manage, organize, view, and filter media and other files on a server such as a home/office NAS

Requirements
* Automate the organization of files such as *.mp3 all go into Music. For example, the automated folder, "Auto". If a file or folder named *.mp3, *.flacc, is dropped into this folder the application will be noted in the database along with metadata and moved into a folder called Music.  

* Provide a web based GUI for management a la FreeNAS.  
* Provide a text based file configuration.  
* Provide a tool to create rulesets based on filename and metadata  
* Allow rulesets to be implemented with POSIX regular expressions  
* Allow the user via a web based GUI to search and filter all files stored on the server.  
* Allow the user to use POSIX style regular expressions to search for files  
* Allow the user to search based on metadata of a file such as Artist in the case of mp3s  
* Provide an option to specify which folders to ignore automatic organization  
* Provide an option to specify which folders to prevent from being stored in the database  

Technical Requirements
  * Use FreeNAS as a starting point but allow other NAS style servers to use this as well  
  * It could start as a FreeNAS plugin  
  * Use a combination of inotify where applicable and polling everywhere else  
  * The application will be written in Python. The frontend web gui will be assisted by Dojango as I am familiar with Dojo and this is what FreeNAS is using
  * The application will initially target any Linux and FreeBSD (supporting Python > 2.7) but consideration for Windows and Mac OSX support should be taken into account during design and implementation
