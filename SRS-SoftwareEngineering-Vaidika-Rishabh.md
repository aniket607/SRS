-   [Software Requirements
    Specifications](#software-requirements-specifications)
    -   [RC Music Player](#rc-music-player)
-   [Table of Contents](#table-of-contents)
-   [1. Introduction](#introduction)
    -   [1.1 Purpose](#purpose)
    -   [1.2 Definitions, Acronyms, and
        Abbreviations](#definitions-acronyms-and-abbreviations)
    -   [1.3 Scope](#scope)
    -   [1.4 Intended Audience](#intended-audience)
    -   [1.5 References](#references)
-   [2. Overall Descriptions](#overall-descriptions)
    -   [2.1 Product Perspective](#product-perspective)
    -   [2.2 Product Functions](#product-functions)
    -   [2.3 User Classes &
        Characteristics](#user-classes--characteristics)
    -   [2.4 Product Constraints](#product-constraints)
    -   [2.5 Use Case Diagram](#use-case-diagram)
    -   [2.6 Class Diagram](#class-diagram)
-   [3. System Features](#system-features)
    -   [3.1 User Interface](#user-interface)
        -   
-   [3.2 Functions / Features](#functions--features)
    -   -   -   

    -   [3.3 Hardware Interfaces](#hardware-interfaces)
    -   [3.4 Software Interfaces](#software-interfaces)
    -   [3.3 Communications Interfaces](#communications-interfaces)

-   [4. Functional & Non-Functional
    Requirements](#functional--non-functional-requirements)
    -   [4.1 Functional Requirements](#functional-requirements)
        -   

    -   [4.2 Non-Functional Requirements](#non-functional-requirements)
-   [5. Testing Methodologies](#testing-methodologies)

Software Requirements Specifications
====================================

RC Music Player
---------------

*version 1.0*

***Prepared by** Vaidika Ranka & Rishabh Singh Tomar, B.Tech II Year,
NMIMS Indore*\
 This document is written in Github flavoured Markdown.

* * * * *

### Brief Description

* * * * *

**Product:** Music Player\
 **Description:** An offline music system\
 **Development Status:** Design phase

### Revisions

* * * * *

    Current Version : 1.0
    Current Status : Work in Progress
    Date : 15-10-2021

Table of Contents
=================

1.  Introduction\
     1.1 Purpose\
     1.2 Definitions, Acronyms, and Abbreviations\
     1.3 Scope\
     1.4 Intended Audience\
     1.5 References
2.  Overall Description\
     2.1 Product Perspective\
     2.2 Product Functions\
     2.3 User Classes and Characteristics\
     2.4 Product Constraints\
     2.5 Use Case Diagram\
     2.6 Class Diagram
3.  System Features\
     3.1 User Interfaces\
     3.2 Hardware Interfaces\
     3.3 Software Interfaces\
     3.4 Communications Interfaces
4.  Functional & Non-Functional Requirements\
     4.1 Functional Requirements\
     4.2 Non-Functional Requirements
5.  Testing Methodologies

1. Introduction
===============

1.1 Purpose
-----------

Τhis Software Requirements Specification document has been created for
the program RC Music Player version 1.0 which is a music player for
playing ordinary audio formats and chiptunes.

RC Music Player is a free, open source program. Free software is
software which may be used, studied, amended and returned without
restriction.

1.2 Definitions, Acronyms, and Abbreviations
--------------------------------------------

As you begin to define a system, you will encounter words which need
definition and general usage acronyms.

These should be documented for new personnel and for clarity of all
concerned parties.\

### 1.3.1 Definitions

*none*\

### 1.3.2 Acronyms

**IEEE** - Institute of Electrical and Electronic Engineers\

### 1.3.3 Abbreviations

*none*

1.3 Scope
---------

RC Music Player is a windows form music player application. It not just
supports modern day audio formats such as MP3 or WAV but also OGG, WMA,
MPC, FLAC and can be expanded by addons. It also supports chiptunes and
plays them like a normal audio file. Next Chapters include extensive
reference to these capabilities of the program.

1.4 Intended Audience
---------------------

-   Anyone with some basic knowledge of programming can understand this
    document. The document is intended for Developers, Software
    architects, Testers, Project managers and Documentation Writers. But
    anyone with programming background and some experience with UML can
    understand this document.

This Software Requirement Specification also includes:

-   Overall description of the product
-   External interface requirements
-   System Features
-   Other non functional requirements

1.5 References
--------------

-   IEEE Software Engineering Standards Committee, “IEEE Std 830-1998,
    IEEE Recommended Practice for Software Requirements Specifications”,
    October 20, 1998.

-   [NoSql Project –
    DjonDB](http://tinman.cs.gsu.edu/~raj/8711/sp13/djondb/Report.pdf)

-   Source for outline of this SRS Document :
    [Wikipedia](https://en.wikipedia.org/wiki/Software_requirements_specification#Structure)\

2. Overall Descriptions
=======================

2.1 Product Perspective
-----------------------

This system consists of two components packaged as one desktop
application:

-   **Music player**: for playing music from local library.
-   **Local Store**: It is implemented as a
    [SQLite](https://www.sqlite.org/) database which acts as a map
    between track titles, paths and keeps a check on each track for its
    metadata information.

The software application will be used to play music and store playlists.
Since this is a data-centric product it will need storage space to store
information of artists, music, playlists, etc. For this purpose, a
database will be made in the user’s machine using SQLite.

The software application will be needing free space for resource
allocation to avoid overloading. The maximum amount of storage space for
the application is 10 megabytes.

The minimum requirements that are needed to run RC Music Player are:

-   **OS:** Windows XP with Service Pack 3 installed.
-   **.NET Framework:** .NET Framework 3.5.
-   **DirectX:** DirectX 3 for audio.
-   **RAM:** 512MB.
-   **Disk Space:** 10MB free space.

2.2 Product Functions
---------------------

Using this app, user can play tracks available in offline library. With
the software application the user can also utilize the following
features:

-   Simple GUI.
-   Full Support For All Audio Formats.
-   Load / Save Playlists.
-   Plays Next / Previous Track On Playlists.
-   Small File Size (Installer is less than 1 MB).
-   Repeat playlists.
-   Enhanced For Windows 7.
-   Output audio clearly on high definition (also depends on your
    system).
-   Hide to tray function to replace the “minimize” button.
-   Unlimited songs on playlist (requires space on the user’s machine).
-   Uses .LRC lyrics format.
-   Tracker to track audio positions and volume.
-   Visualizes Window’s Aero (Windows 7 only).
-   Mixer to set DX8 effects on the current playing audio.
-   Simple Tags editor to edit title, artist and album.
-   Shows left / right audio volume.
-   Simple interface.
-   Console (CMD) interface.

2.3 User Classes & Characteristics {#user-classes--characteristics}
----------------------------------

The software can be used by the following user categories:

-   Almost any user will be able to easily get going with this
    application as it is perfectly meant for an average music lover.
    Music lovers especially interested in playing various genres of
    music in a playlist for background music playing for instance will
    be benefited more than ever by this application as it does not
    require the internet for playing the music.
-   Simple users that intend to hear a song. These users could be of any
    age, with no special knowledge. Knowing how to use a computer is
    essential.
-   Users with poor internet connectivity will benefit even more because
    the only place we require internet connection is where we are
    required to update the metadata of the music for giving correct
    suggestions.
-   Programmers - Software Developers – Open Source project participants
    of any age that could understand the program’s source code and
    expand or improve it. Must have knowledge of the programming
    language that the software is written in, in order to be able to
    understand exactly what it does and how it does it. Also some
    experience in programming will most certainly help in extending or
    improving the project.

There is no restriction in user’s categories and everyone using a
computer can use this program.

This is an Open Source project and anyone who desires to distribute to
the project is welcome.

2.4 Product Constraints
-----------------------

Software application needs to have an operating system that has enough
performance. If the operating system does not have enough hardware
resources available for the application. Then, there may be scenarios
where the application does not work as intended or even at all.

2.5 Use Case Diagram
--------------------

Following is the use case diagram of our system.\
 ![Usecase Diagram for RC Music
Player](https://user-images.githubusercontent.com/90885153/137472929-cc9bedd5-7573-479a-b99d-d012fb18b8ef.png)\
 RC Music Player being an offline player is independent of any admin.
The user can and does manages the entire system by themselves.

Broadly, the user has three component to run:

-   **Control Music:** Using this functionality, the user can play
    music, seek to a part of the song, stop the playing song, control
    the volume, pause the song, and change the tracks.
-   **Edit Metadata:** Metadata of the albums, songs, playlists, etc.
    This then works together with Local Storage to modify the metadata.
-   **Manage Songs:** Add songs and remove songs from the system. With
    the version 2.0, we are planning to implement a system where the
    player automatically detects files that can played with out system.
    Until that, the user has to manually add and delete songs into the
    system.

Use Case Description table

  Use Case Title                Description
  ----------------------------- -----------------------------------------------------
  *Manage Songs*                generalization of Manage songs
  *Control Music*               generalization of control songs
  *Edit Metadata*               user edits metadata
  *Control Volume*              use controls volume
  *Play*                        user can play music
  *Pause*                       user can pause
  *Seek*                        user can seek into timeline of playing track
  *Stop*                        user can stop the playing track
  *Next Track*                  user can change to next track
  *Previous Track*              user can go to previous track
  *Add songs*                   user can add songs
  *Remove Songs*                user can remove songs from list
  *Access Local Storage*        components can access local storage for persistence
  *Read from local Storage*     components can read from local storage
  *Write into local Storage*    components can write into local storage
  *Update into local Storage*   components can update data into local storage
  *Delete from local Storage*   components can delete items from local storage

2.6 Class Diagram
-----------------

![Untitled
Diagram](https://user-images.githubusercontent.com/90885153/137478087-0f4c8f2f-1ae0-4b45-9360-16517d8a866e.png)\
 RC Music Player will work need 5 independent classes, namely:

-   **Metadata Class:** This class will deal with the metadata of songs,
    playlists, etc.
-   **Player Class:** This class will deal with the player options. It
    can seek the music forward, it can change the tracks, it will
    display the information of the track playing, etc. Everything that’s
    going on the screen is dealt by this class.
-   **Permission Class:** This class has no direct relationship with the
    working of our system, but this helps in maintaining the abstraction
    for our system.
-   **Track Class:** This class contains all the information about the
    tracks. It works with player class to display the information on the
    screen.
-   **File Handling Class:** This is the fundamental class for the
    system. It helps in storing the playlists, music, track information,
    genre, metadata, queue, etc to the system. This works with SQLite to
    read and write information to the user system.

3. System Features
==================

The system features and functional requirements are described in detail,
to help the reader understand the application better and developers and
testers in their future work in RC Music Player.

3.1 User Interface
------------------

#### Mock UI (Main Screen)

* * * * *

![Kasoor
(1)](https://user-images.githubusercontent.com/90885153/137502738-e173fa01-3d83-4806-948c-ff51e2096248.png)

#### Mock UI (Player Screen)

* * * * *

![Kasoor
(2)](https://user-images.githubusercontent.com/90885153/137502909-f70660c8-5135-4899-aa2f-9782282d1b45.png)

1.  ***Title Bar*** – shows song length and position.

2.  ***Menu Bar*** - contains “File”, “View”, “Tools” and “Help”.

3.  ***Left Progress Bar*** - shows volume on the left speaker.

4.  ***Right Progress Bar*** - shows the volume on the right speaker.

5.  ***Previous Button*** - switch to the previous song in the playlist

6.  ***Pause Button*** - temporarily stops the current playing audio.

7.  ***Play Button*** - plays and resumes the paused audio.

8.  ***Next Button*** - switch to the next song in the playlist.

9.  ***File*** - contains important functions such as “Add”, “Add From
    URL”, etc.

10. ***View*** - contains optional functions such as “Visualizations”,
    “Repeat”, etc.

11. ***Tools*** - contains editing tools such as “Tags Editor”,
    “Playlist Tool”, “Console”, Etc.

12. ***Help*** - contains support and information about the program.

13. ***Toolbar*** - contains playing functions such as “Play”, “Pause”,
    “Stop”, etc.

3.2 Functions / Features {#functions--features}
========================

**Add Media To Playlist**

With this choice, users can choose a song from the hard disk and add it
to the playlist. When a user chooses the file then this will start
playing automatically.

##### Play

With this operation the chosen song starts playing. If there are no
registered records in the playlist when users choose Play, then the user
has the opportunity to choose songs from the disk automatically.

##### Pause

This choice interrupts the song and if the user chooses Play then the
song starts playing from the same point.

##### Stop

With this choice the song stops playing. If the user chooses the choice
Play the file will start to play from the beginning.

##### Previous on Playlist

With this choice the previous song on the playlist is chosen
automatically and starts playing.

##### Next on Playlist

With this choice the next song on the playlist is chosen automatically
and starts playing.

##### Volume Up

This choice is to increase the sound.

##### Volume Down

This choice is to decrease the sound.

##### Exit

With this choice users can close the RC Music Player. This choice closes
the program.

##### Playlist

This choice pops up a new window where songs are to be played.

##### Music Information Ctrl+I

With this choice appear two new windows with all the information for the
current file sound. Specifically the window album cover art shows the
image of the cover of album and the second window shows the following
information:

-   title

-   artist

-   album

-   album artist

-   composer

-   track

-   type

-   year

-   comments

3.3 Hardware Interfaces
-----------------------

-   Music player needs playback device for sound output.

3.4 Software Interfaces
-----------------------

These are the minimum requirements that are needed to run and build RC
Music Player

-   ***OS:*** Windows XP with Service Pack 3 installed.

-   ***.NET Framework:*** .NET Framework 3.5.

-   ***DirectX:*** DirectX 3 for audio.

-   ***RAM:*** 512MB.

-   ***Disk Space:*** 10MB free space.

3.3 Communications Interfaces
-----------------------------

NONE

4. Functional & Non-Functional Requirements {#functional--non-functional-requirements}
===========================================

4.1 Functional Requirements
---------------------------

  **Functional Requirement Name**   **Description**
  --------------------------------- ----------------------------------------------------------------------------------------------------------------------------------
  Manually update metadata          The user will be able to update the metadata of any track manually, i.e., simply by right clicking
  Volume control                    The user will be able to increase or decrease or mute the volume of the playing track
  Play music                        The user will be able to play the track by selecting it or clicking on Play
  Pause music                       The user will be able to pause the track being able to play it again from the same timeline
  Seek track                        The user will be able to move anywhere in the timeline of the track
  Stop music                        The user will be able to stop the track which will close the track, in order for the user to play another track or exit software
  Go to the next track              The user will be able to play the next track
  Go to the previous track          The user will be able to play the previous track
  Add songs                         The user will be able to import music from his external music collection, to the application
  Remove songs                      The user will be able to remove any track from the playlist

#### Music player

Built into the RC Music Player is a music player that can play music
with a number of controls including **play, pause, stop, play next or
previous track, seek and volume control**.

-   The user will be able to import music from his offline music
    collection which may simply refer to a hard-drive or a flash memory.

-   In import stage software will build an Internal Local Store with
    Information about added tracks.

-   User can remove a track from imported music and that will remove the
    corresponding entry from Local Store

#### Local Store

Local Store is persistence layer of application, it will be implemented
as SQLite Database. It will store all the information required for
software to work

-   The user will be able to essentially cache data into a local store
    while importing a track into the application.

-   On adding a track or importing a track from the offline music
    library of the user to the application the track will be added into
    the local store.

-   On removing the track from the application the track will also be
    removed from the Local store. In short the Local store maintains the
    library of the application.

-   It will not be available for user to direct interaction, This
    component will be used by other components internally.

#### User actions

This section will state all the use cases of the application and what
the user will be able to do with the application.

-   **Music management**

> The user will be able to manage music, import and export. The user
> will be able to import music files from offline music collection and
> also remove music files from the application.

-   **Control music**

> The user can control music in the music player component by the
> following actions:
>
> -   play music
> -   pause music
> -   control volume
> -   go to the next track
> -   go to the previous track
> -   seek a playing track

-   **manual updation of metadata**

> The user will be able to manage metadata of the tracks that he/she
> chooses.

#### User Interactions

The following are the use cases and how the actor: user interacts with
them

**Use case: Manage tracks**

**Brief Description**

The user manages tracks, can import and remove them from the application

**User interaction**

-   Import tracks from offline music collection
-   Add directories, sub directories and files to the music player.
-   The user can remove the track from the application
-   The local store updates itself deleting the track

**Use case: Control Music**

**Brief Description**

The user can control music which means he/she can play, pause, stop, go
to the next track, go to the previous track, control the volume

**User interaction**

-   Click events trigger all controlling of music operations.

**Use case: Edit metadata**

**Brief Description**

The user can also manually edit his/her track’s metadata

**User interaction**

-   The user defined metadata of a track is going to be updated in the
    local store.

4.2 Non-Functional Requirements
-------------------------------

The non-functional requirements of the system are explained below.

### 4.2.1 Performance Requirements

RC Music Player requires a small amount of disk space for
installation-10MB. It is characterized by fast loading and executing
times. It‘s not a heavy program and it can work while other programs are
running.

-   **Quickness**

    -   System should be fast enough to play music and respond to any of
        the user action in any way without any shattering or buffering,
        else it will be not be a good experience.
-   **Robustness**

    -   System should be robust to deal and act accordingly with common
        error scenarios like unavailable metadata, unsupported file
        types, etc.
-   **Failure Handling**

    -   In case of failures it should be able to fail or recover
        quickly.

### 4.2.2 Safety Requirements

-   **Exception Handling**

    -   The software should be able to restrict or warn(in the first
        place) the user from doing things not suitable, like, increasing
        volume beyond threshold, or exiting the software w/o saving the
        changed data.

### 4.2.3 Software Quality Attributes

RC Music Player is easy to use because it is a small program. Users can
easily learn to use it. The software’s interface is quite friendly,
simple, easily understood, it works fast and is organized. RC Music
Player is a very fast and efficient program and users can easily change
its options to satisfy their needs. Some Software Quality Attributes of
RC Music Player are:

-   **Memory Management**

    -   System should not leak memory.
-   **Compatibility**

    -   System should peacefully co-exist with other software
-   **Error Handling**

    -   System should not cause or trigger any events that will leave
        Operating System in unrecoverable state

5. Testing Methodologies
========================

* * * * *
