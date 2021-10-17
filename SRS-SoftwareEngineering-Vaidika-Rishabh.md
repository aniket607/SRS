<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>SRS-SoftwareEngineering-Vaidika-Rishabh</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__left">
    <div class="stackedit__toc">
      
<ul>
<li><a href="#software-requirements-specifications">Software Requirements Specifications</a>
<ul>
<li><a href="#rc-music-player">RC Music Player</a></li>
</ul>
</li>
<li><a href="#table-of-contents">Table of Contents</a></li>
<li><a href="#introduction">1. Introduction</a>
<ul>
<li><a href="#purpose">1.1 Purpose</a></li>
<li><a href="#definitions-acronyms-and-abbreviations">1.2 Definitions, Acronyms, and Abbreviations</a></li>
<li><a href="#scope">1.3 Scope</a></li>
<li><a href="#intended-audience">1.4 Intended Audience</a></li>
<li><a href="#references">1.5 References</a></li>
</ul>
</li>
<li><a href="#overall-descriptions">2. Overall Descriptions</a>
<ul>
<li><a href="#product-perspective">2.1 Product Perspective</a></li>
<li><a href="#product-functions">2.2 Product Functions</a></li>
<li><a href="#user-classes--characteristics">2.3 User Classes & Characteristics</a></li>
<li><a href="#product-constraints">2.4 Product Constraints</a></li>
<li><a href="#use-case-diagram">2.5 Use Case Diagram</a></li>
<li><a href="#class-diagram">2.6 Class Diagram</a></li>
</ul>
</li>
<li><a href="#system-features">3. System Features</a>
<ul>
<li><a href="#user-interface">3.1 User Interface</a>
<ul>
<li></li>
</ul>
</li>
</ul>
</li>
<li><a href="#functions--features">3.2 Functions / Features</a>
<ul>
<li>
<ul>
<li>
<ul>
<li></li>
</ul>
</li>
</ul>
</li>
<li><a href="#hardware-interfaces">3.3 Hardware Interfaces</a></li>
<li><a href="#software-interfaces">3.4 Software Interfaces</a></li>
<li><a href="#communications-interfaces">3.3 Communications Interfaces</a></li>
</ul>
</li>
<li><a href="#functional--non-functional-requirements">4. Functional & Non-Functional Requirements</a>
<ul>
<li><a href="#functional-requirements">4.1 Functional Requirements</a>
<ul>
<li></li>
</ul>
</li>
<li><a href="#non-functional-requirements">4.2 Non-Functional Requirements</a></li>
</ul>
</li>
<li><a href="#testing-methodologies">5. Testing Methodologies</a></li>
</ul>

    </div>
  </div>
  <div class="stackedit__right">
    <div class="stackedit__html">
      <h1 id="software-requirements-specifications">Software Requirements Specifications</h1>
<h2 id="rc-music-player">RC Music Player</h2>
<p><em>version 1.0</em></p>
<p><em><strong>Prepared by</strong> Vaidika Ranka &amp; Rishabh Singh Tomar, B.Tech II Year, NMIMS Indore</em><br>
This document is written in Github flavoured Markdown.</p>
<hr>
<h3 id="brief-description">Brief Description</h3>
<hr>
<p><strong>Product:</strong> Music Player<br>
<strong>Description:</strong> An offline music system<br>
<strong>Development Status:</strong> Design phase</p>
<h3 id="revisions">Revisions</h3>
<hr>
<pre><code>Current Version : 1.0
Current Status : Work in Progress
Date : 15-10-2021
</code></pre>
<h1 id="table-of-contents">Table of Contents</h1>
<ol>
<li>Introduction<br>
1.1  Purpose<br>
1.2  Definitions, Acronyms, and Abbreviations<br>
1.3  Scope<br>
1.4  Intended Audience<br>
1.5  References</li>
<li>Overall Description<br>
2.1  Product Perspective<br>
2.2  Product Functions<br>
2.3  User Classes and Characteristics<br>
2.4  Product Constraints<br>
2.5  Use Case Diagram<br>
2.6 Class Diagram</li>
<li>System Features<br>
3.1  User Interfaces<br>
3.2  Hardware Interfaces<br>
3.3  Software Interfaces<br>
3.4  Communications Interfaces</li>
<li>Functional &amp; Non-Functional Requirements<br>
4.1 Functional Requirements<br>
4.2 Non-Functional Requirements</li>
<li>Testing Methodologies</li>
</ol>
<h1 id="introduction">1. Introduction</h1>
<p><a></a></p>
<h2 id="purpose">1.1 Purpose</h2>
<p>Τhis Software Requirements Specification document has been created for the program RC Music Player version 1.0 which is a music player for playing ordinary audio formats and chiptunes.</p>
<p>RC Music Player is a free, open source program. Free software is software which may be used, studied, amended and returned without restriction.</p>
<p><a></a></p>
<h2 id="definitions-acronyms-and-abbreviations">1.2 Definitions, Acronyms, and Abbreviations</h2>
<p>As you begin to define a system, you will encounter words which need definition and general usage acronyms.</p>
<p>These should be documented for new personnel and for clarity of all concerned parties.<br>
<a></a></p>
<h3 id="definitions">1.3.1 Definitions</h3>
<p><em>none</em><br>
<a></a></p>
<h3 id="acronyms">1.3.2 Acronyms</h3>
<p><strong>IEEE</strong> - Institute of Electrical and Electronic Engineers<br>
<a></a></p>
<h3 id="abbreviations">1.3.3 Abbreviations</h3>
<p><em>none</em></p>
<p><a></a></p>
<h2 id="scope">1.3 Scope</h2>
<p>RC Music Player is a windows form music player application. It not just supports modern day audio formats such as MP3 or WAV but also OGG, WMA, MPC, FLAC and can be expanded by addons. It also supports chiptunes and plays them like a normal audio file. Next Chapters include extensive reference to these capabilities of the program.</p>
<p><a></a></p>
<h2 id="intended-audience">1.4 Intended Audience</h2>
<ul>
<li>Anyone with some basic knowledge of programming can understand this document. The document is intended for Developers, Software architects, Testers, Project managers and Documentation Writers. But anyone with programming background and some experience with UML can understand this document.</li>
</ul>
<p>This Software Requirement Specification also includes:</p>
<ul>
<li>Overall description of the product</li>
<li>External interface requirements</li>
<li>System Features</li>
<li>Other non functional requirements</li>
</ul>
<p><a></a></p>
<h2 id="references">1.5 References</h2>
<ul>
<li>
<p>IEEE Software Engineering Standards Committee, “IEEE Std 830-1998, IEEE Recommended Practice for Software Requirements Specifications”, October 20, 1998.</p>
</li>
<li>
<p><a href="http://tinman.cs.gsu.edu/~raj/8711/sp13/djondb/Report.pdf">NoSql Project – DjonDB</a></p>
</li>
<li>
<p>Source for outline of this SRS Document :  <a href="https://en.wikipedia.org/wiki/Software_requirements_specification#Structure">Wikipedia</a><br>
<a></a></p>
</li>
</ul>
<h1 id="overall-descriptions">2. Overall Descriptions</h1>
<p><a></a></p>
<h2 id="product-perspective">2.1 Product Perspective</h2>
<p>This system consists of two components packaged as one desktop application:</p>
<ul>
<li><strong>Music player</strong>: for playing music from local library.</li>
<li><strong>Local Store</strong>: It is implemented as a  <a href="https://www.sqlite.org/">SQLite</a>  database which acts as a map between track titles, paths and keeps a check on each track for its metadata information.</li>
</ul>
<p>The software application will be used to play music and store playlists. Since this is a data-centric product it will need storage space to store information of artists, music, playlists, etc. For this purpose, a database will be made in the user’s machine using SQLite.</p>
<p>The software application will be needing free space for resource allocation to avoid overloading. The maximum amount of storage space for the application is 10 megabytes.</p>
<p>The minimum requirements that are needed to run RC Music Player are:</p>
<ul>
<li><strong>OS:</strong>  Windows XP with Service Pack 3 installed.</li>
<li><strong>.NET Framework:</strong>  .NET Framework 3.5.</li>
<li><strong>DirectX:</strong>  DirectX 3 for audio.</li>
<li><strong>RAM:</strong>  512MB.</li>
<li><strong>Disk Space:</strong>  10MB free space.</li>
</ul>
<p><a></a></p>
<h2 id="product-functions">2.2 Product Functions</h2>
<p>Using this app, user can play tracks available in offline library. With the software application the user can also utilize the following features:</p>
<ul>
<li>Simple GUI.</li>
<li>Full Support For All Audio Formats.</li>
<li>Load / Save Playlists.</li>
<li>Plays Next / Previous Track On Playlists.</li>
<li>Small File Size (Installer is less than 1 MB).</li>
<li>Repeat playlists.</li>
<li>Enhanced For Windows 7.</li>
<li>Output audio clearly on high definition (also depends on your system).</li>
<li>Hide to tray function to replace the “minimize” button.</li>
<li>Unlimited songs on playlist (requires space on the user’s machine).</li>
<li>Uses .LRC lyrics format.</li>
<li>Tracker to track audio positions and volume.</li>
<li>Visualizes Window’s Aero (Windows 7 only).</li>
<li>Mixer to set DX8 effects on the current playing audio.</li>
<li>Simple Tags editor to edit title, artist and album.</li>
<li>Shows left / right audio volume.</li>
<li>Simple interface.</li>
<li>Console (CMD) interface.</li>
</ul>
<p><a></a></p>
<h2 id="user-classes--characteristics">2.3 User Classes &amp; Characteristics</h2>
<p>The software can be used by the following user categories:</p>
<ul>
<li>Almost any user will be able to easily get going with this application as it is perfectly meant for an average music lover. Music lovers especially interested in playing various genres of music in a playlist for background music playing for instance will be benefited more than ever by this application as it does not require the internet for playing the music.</li>
<li>Simple users that intend to hear a song. These users could be of any age, with no special knowledge. Knowing how to use a computer is essential.</li>
<li>Users with poor internet connectivity will benefit even more because the only place we require internet connection is where we are required to update the metadata of the music for giving correct suggestions.</li>
<li>Programmers - Software Developers – Open Source project participants of any age that could understand the program’s source code and expand or improve it. Must have knowledge of the programming language that the software is written in, in order to be able to understand exactly what it does and how it does it. Also some experience in programming will most certainly help in extending or improving the project.</li>
</ul>
<p>There is no restriction in user’s categories and everyone using a computer can use this program.</p>
<p>This is an Open Source project and anyone who desires to distribute to the project is welcome.</p>
<p><a></a></p>
<h2 id="product-constraints">2.4 Product Constraints</h2>
<p>Software application needs to have an operating system that has enough performance. If the operating system does not have enough hardware resources available for the application. Then, there may be scenarios where the application does not work as intended or even at all.</p>
<p><a></a></p>
<h2 id="use-case-diagram">2.5 Use Case Diagram</h2>
<p>Following is the use case diagram of our system.<br>
<img src="https://user-images.githubusercontent.com/90885153/137472929-cc9bedd5-7573-479a-b99d-d012fb18b8ef.png" alt="Usecase Diagram for RC Music Player"><br>
RC Music Player being an offline player is independent of any admin. The user can and does manages the entire system by themselves.</p>
<p>Broadly, the user has three component to run:</p>
<ul>
<li><strong>Control Music:</strong>  Using this functionality, the user can play music, seek to a part of the song, stop the playing song, control the volume, pause the song, and change the tracks.</li>
<li><strong>Edit Metadata:</strong> Metadata of the albums, songs, playlists, etc. This then works together with Local Storage to modify the metadata.</li>
<li><strong>Manage Songs:</strong> Add songs and remove songs from the system. With the version 2.0, we are planning to implement a system where the player automatically detects files that can played with out system. Until that, the user has to manually add and delete songs into the system.</li>
</ul>
<p>Use Case Description table</p>

<table>
<thead>
<tr>
<th>Use Case Title</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><em>Manage Songs</em></td>
<td>generalization of Manage songs</td>
</tr>
<tr>
<td><em>Control Music</em></td>
<td>generalization of control songs</td>
</tr>
<tr>
<td><em>Edit Metadata</em></td>
<td>user edits metadata</td>
</tr>
<tr>
<td><em>Control Volume</em></td>
<td>use controls volume</td>
</tr>
<tr>
<td><em>Play</em></td>
<td>user can play music</td>
</tr>
<tr>
<td><em>Pause</em></td>
<td>user can pause</td>
</tr>
<tr>
<td><em>Seek</em></td>
<td>user can seek into timeline of playing track</td>
</tr>
<tr>
<td><em>Stop</em></td>
<td>user can stop the playing track</td>
</tr>
<tr>
<td><em>Next Track</em></td>
<td>user can change to next track</td>
</tr>
<tr>
<td><em>Previous Track</em></td>
<td>user can go to previous track</td>
</tr>
<tr>
<td><em>Add songs</em></td>
<td>user can add songs</td>
</tr>
<tr>
<td><em>Remove Songs</em></td>
<td>user can remove songs from list</td>
</tr>
<tr>
<td><em>Access Local Storage</em></td>
<td>components can access local storage for persistence</td>
</tr>
<tr>
<td><em>Read from local Storage</em></td>
<td>components can read from local storage</td>
</tr>
<tr>
<td><em>Write into local Storage</em></td>
<td>components can write into local storage</td>
</tr>
<tr>
<td><em>Update into local Storage</em></td>
<td>components can update data into local storage</td>
</tr>
<tr>
<td><em>Delete from local Storage</em></td>
<td>components can delete items from local storage</td>
</tr>
</tbody>
</table><p><a></a></p>
<h2 id="class-diagram">2.6 Class Diagram</h2>
<p><img src="https://user-images.githubusercontent.com/90885153/137478087-0f4c8f2f-1ae0-4b45-9360-16517d8a866e.png" alt="Untitled Diagram"><br>
RC Music Player will work need 5 independent classes, namely:</p>
<ul>
<li><strong>Metadata Class:</strong> This class will deal with the metadata of songs, playlists, etc.</li>
<li><strong>Player Class:</strong> This class will deal with the player options. It can seek the music forward, it can change the tracks, it will display the information of the track playing, etc. Everything that’s going on the screen is dealt by this class.</li>
<li><strong>Permission Class:</strong> This class has no direct relationship with the working of our system, but this helps in maintaining the abstraction for our system.</li>
<li><strong>Track Class:</strong> This class contains all the information about the tracks. It works with player class to display the information on the screen.</li>
<li><strong>File Handling Class:</strong> This is the fundamental class for the system. It helps in storing the playlists, music, track information, genre, metadata, queue, etc to the system. This works with SQLite to read and write information to the user system.</li>
</ul>
<p><a></a></p>
<h1 id="system-features">3. System Features</h1>
<p>The system features and functional requirements are described in detail, to help the reader understand the application better and developers and testers in their future work in RC Music Player.</p>
<p><a></a></p>
<h2 id="user-interface">3.1 User Interface</h2>
<h4 id="mock-ui-main-screen">Mock UI (Main Screen)</h4>
<hr>
<p><img src="https://user-images.githubusercontent.com/90885153/137502738-e173fa01-3d83-4806-948c-ff51e2096248.png" alt="Kasoor (1)"></p>
<h4 id="mock-ui-player-screen">Mock UI (Player Screen)</h4>
<hr>
<p><img src="https://user-images.githubusercontent.com/90885153/137502909-f70660c8-5135-4899-aa2f-9782282d1b45.png" alt="Kasoor (2)"></p>
<ol>
<li>
<p><em><strong>Title Bar</strong></em> – shows song length and position.</p>
</li>
<li>
<p><em><strong>Menu Bar</strong></em> - contains “File”, “View”, “Tools” and “Help”.</p>
</li>
<li>
<p><em><strong>Left Progress Bar</strong></em> - shows volume on the left speaker.</p>
</li>
<li>
<p><em><strong>Right Progress Bar</strong></em> - shows the volume on the right speaker.</p>
</li>
<li>
<p><em><strong>Previous Button</strong></em> - switch to the previous song in the playlist</p>
</li>
<li>
<p><em><strong>Pause Button</strong></em> - temporarily stops the current playing audio.</p>
</li>
<li>
<p><em><strong>Play Button</strong></em> - plays and resumes the paused audio.</p>
</li>
<li>
<p><em><strong>Next Button</strong></em> - switch to the next song in the playlist.</p>
</li>
<li>
<p><em><strong>File</strong></em> - contains important functions such as “Add”, “Add From URL”, etc.</p>
</li>
<li>
<p><em><strong>View</strong></em> - contains optional functions such as “Visualizations”, “Repeat”, etc.</p>
</li>
<li>
<p><em><strong>Tools</strong></em> - contains editing tools such as “Tags Editor”, “Playlist Tool”, “Console”, Etc.</p>
</li>
<li>
<p><em><strong>Help</strong></em> - contains support and information about the program.</p>
</li>
<li>
<p><em><strong>Toolbar</strong></em> - contains playing functions such as “Play”, “Pause”, “Stop”, etc.</p>
</li>
</ol>
<p><a></a></p>
<h1 id="functions--features">3.2 Functions / Features</h1>
<p><strong>Add Media To Playlist</strong></p>
<p>With this choice, users can choose a song from the hard disk and add it to the playlist. When a user chooses the file then this will start playing automatically.</p>
<h5 id="play">Play</h5>
<p>With this operation the chosen song starts playing. If there are no registered records in the playlist when users choose Play, then the user has the opportunity to choose songs from the disk automatically.</p>
<h5 id="pause">Pause</h5>
<p>This choice interrupts the song and if the user chooses Play then the song starts playing from the same point.</p>
<h5 id="stop">Stop</h5>
<p>With this choice the song stops playing. If the user chooses the choice Play the file will start to play from the beginning.</p>
<h5 id="previous-on-playlist">Previous on Playlist</h5>
<p>With this choice the previous song on the playlist is chosen automatically and starts playing.</p>
<h5 id="next-on-playlist">Next on Playlist</h5>
<p>With this choice the next song on the playlist is chosen automatically and starts playing.</p>
<h5 id="volume-up">Volume Up</h5>
<p>This choice is to increase the sound.</p>
<h5 id="volume-down">Volume Down</h5>
<p>This choice is to decrease the sound.</p>
<h5 id="exit">Exit</h5>
<p>With this choice users can close the RC Music Player. This choice closes the program.</p>
<h5 id="playlist">Playlist</h5>
<p>This choice pops up a new window where songs are to be played.</p>
<h5 id="music-information-ctrli">Music Information Ctrl+I</h5>
<p>With this choice appear two new windows with all the information for the current file sound. Specifically the window album cover art shows the image of the cover of album and the second window shows the following information:</p>
<ul>
<li>
<p>title</p>
</li>
<li>
<p>artist</p>
</li>
<li>
<p>album</p>
</li>
<li>
<p>album artist</p>
</li>
<li>
<p>composer</p>
</li>
<li>
<p>track</p>
</li>
<li>
<p>type</p>
</li>
<li>
<p>year</p>
</li>
<li>
<p>comments</p>
</li>
</ul>
<p><a></a></p>
<h2 id="hardware-interfaces">3.3 Hardware Interfaces</h2>
<ul>
<li>Music player needs playback device for sound output.</li>
</ul>
<p><a></a></p>
<h2 id="software-interfaces">3.4 Software Interfaces</h2>
<p>These are the minimum requirements that are needed to run and build RC Music Player</p>
<ul>
<li>
<p><em><strong>OS:</strong></em> Windows XP with Service Pack 3 installed.</p>
</li>
<li>
<p><em><strong>.NET Framework:</strong></em> .NET Framework 3.5.</p>
</li>
<li>
<p><em><strong>DirectX:</strong></em> DirectX 3 for audio.</p>
</li>
<li>
<p><em><strong>RAM:</strong></em> 512MB.</p>
</li>
<li>
<p><em><strong>Disk Space:</strong></em> 10MB free space.</p>
</li>
</ul>
<p><a></a></p>
<h2 id="communications-interfaces">3.3 Communications Interfaces</h2>
<p>NONE</p>
<p><a></a></p>
<h1 id="functional--non-functional-requirements">4. Functional &amp; Non-Functional Requirements</h1>
<p><a></a></p>
<h2 id="functional-requirements">4.1 Functional Requirements</h2>

<table>
<thead>
<tr>
<th><strong>Functional Requirement Name</strong></th>
<th><strong>Description</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>Manually update metadata</td>
<td>The user will be able to update the metadata of any track manually, i.e., simply by right clicking</td>
</tr>
<tr>
<td>Volume control</td>
<td>The user will be able to increase or decrease or mute the volume of the playing track</td>
</tr>
<tr>
<td>Play music</td>
<td>The user will be able to play the track by selecting it or clicking on Play</td>
</tr>
<tr>
<td>Pause music</td>
<td>The user will be able to pause the track being able to play it again from the same timeline</td>
</tr>
<tr>
<td>Seek track</td>
<td>The user will be able to move anywhere in the timeline of the track</td>
</tr>
<tr>
<td>Stop music</td>
<td>The user will be able to stop the track which will close the track, in order for the user to play another track or exit software</td>
</tr>
<tr>
<td>Go to the next track</td>
<td>The user will be able to play the next track</td>
</tr>
<tr>
<td>Go to the previous track</td>
<td>The user will be able to play the previous track</td>
</tr>
<tr>
<td>Add songs</td>
<td>The user will be able to import music from his external music collection, to the application</td>
</tr>
<tr>
<td>Remove songs</td>
<td>The user will be able to remove any track from the playlist</td>
</tr>
</tbody>
</table><h4 id="music-player">Music player</h4>
<p>Built into the RC Music Player is a music player that can play music with a number of controls including  <strong>play, pause, stop, play next or previous track, seek and volume control</strong>.</p>
<ul>
<li>
<p>The user will be able to import music from his offline music collection which may simply refer to a hard-drive or a flash memory.</p>
</li>
<li>
<p>In import stage software will build an Internal Local Store with Information about added tracks.</p>
</li>
<li>
<p>User can remove a track from imported music and that will remove the corresponding entry from Local Store</p>
</li>
</ul>
<h4 id="local-store">Local Store</h4>
<p>Local Store is persistence layer of application, it will be implemented as SQLite Database. It will store all the information required for software to work</p>
<ul>
<li>
<p>The user will be able to essentially cache data into a local store while importing a track into the application.</p>
</li>
<li>
<p>On adding a track or importing a track from the offline music library of the user to the application the track will be added into the local store.</p>
</li>
<li>
<p>On removing the track from the application the track will also be removed from the Local store. In short the Local store maintains the library of the application.</p>
</li>
<li>
<p>It will not be available for user to direct interaction, This component will be used by other components internally.</p>
</li>
</ul>
<h4 id="user-actions">User actions</h4>
<p>This section will state all the use cases of the application and what the user will be able to do with the application.</p>
<ul>
<li><strong>Music management</strong></li>
</ul>
<blockquote>
<p>The user will be able to manage music, import and export. The user will be able to import music files from offline music collection and also remove music files from the application.</p>
</blockquote>
<ul>
<li><strong>Control music</strong></li>
</ul>
<blockquote>
<p>The user can control music in the music player component by the following actions:</p>
<ul>
<li>play music</li>
<li>pause music</li>
<li>control volume</li>
<li>go to the next track</li>
<li>go to the previous track</li>
<li>seek a playing track</li>
</ul>
</blockquote>
<ul>
<li><strong>manual updation of metadata</strong></li>
</ul>
<blockquote>
<p>The user will be able to manage metadata of the tracks that he/she chooses.</p>
</blockquote>
<h4 id="user-interactions">User Interactions</h4>
<p>The following are the use cases and how the actor: user interacts with them</p>
<p><strong>Use case: Manage tracks</strong></p>
<p><strong>Brief Description</strong></p>
<p>The user manages tracks, can import and remove them from the application</p>
<p><strong>User interaction</strong></p>
<ul>
<li>Import tracks from offline music collection</li>
<li>Add directories, sub directories and files to the music player.</li>
<li>The user can remove the track from the application</li>
<li>The local store updates itself deleting the track</li>
</ul>
<p><strong>Use case: Control Music</strong></p>
<p><strong>Brief Description</strong></p>
<p>The user can control music which means he/she can play, pause, stop, go to the next track, go to the previous track, control the volume</p>
<p><strong>User interaction</strong></p>
<ul>
<li>Click events trigger all controlling of music operations.</li>
</ul>
<p><strong>Use case: Edit metadata</strong></p>
<p><strong>Brief Description</strong></p>
<p>The user can also manually edit his/her track’s metadata</p>
<p><strong>User interaction</strong></p>
<ul>
<li>The user defined metadata of a track is going to be updated in the local store.</li>
</ul>
<p><a></a></p>
<h2 id="non-functional-requirements">4.2 Non-Functional Requirements</h2>
<p>The non-functional requirements of the system are explained below.</p>
<h3 id="performance-requirements">4.2.1 Performance Requirements</h3>
<p>RC Music Player requires a small amount of disk space for installation-10MB. It is characterized by fast loading and executing times. It‘s not a heavy program and it can work while other programs are running.</p>
<ul>
<li>
<p><strong>Quickness</strong></p>
<ul>
<li>System should be fast enough to play music and respond to any of the user action in any way without any shattering or buffering, else it will be not be a good experience.</li>
</ul>
</li>
<li>
<p><strong>Robustness</strong></p>
<ul>
<li>System should be robust to deal and act accordingly with common error scenarios like unavailable metadata, unsupported file types, etc.</li>
</ul>
</li>
<li>
<p><strong>Failure Handling</strong></p>
<ul>
<li>In case of failures it should be able to fail or recover quickly.</li>
</ul>
</li>
</ul>
<h3 id="safety-requirements">4.2.2 Safety Requirements</h3>
<ul>
<li>
<p><strong>Exception Handling</strong></p>
<ul>
<li>The software should be able to restrict or warn(in the first place) the user from doing things not suitable, like, increasing volume beyond threshold, or exiting the software w/o saving the changed data.</li>
</ul>
</li>
</ul>
<h3 id="software-quality-attributes">4.2.3 Software Quality Attributes</h3>
<p>RC Music Player is easy to use because it is a small program. Users can easily learn to use it. The software’s interface is quite friendly, simple, easily understood, it works fast and is organized. RC Music Player is a very fast and efficient program and users can easily change its options to satisfy their needs. Some Software Quality Attributes of RC Music Player are:</p>
<ul>
<li>
<p><strong>Memory Management</strong></p>
<ul>
<li>System should not leak memory.</li>
</ul>
</li>
<li>
<p><strong>Compatibility</strong></p>
<ul>
<li>System should peacefully co-exist with other software</li>
</ul>
</li>
<li>
<p><strong>Error Handling</strong></p>
<ul>
<li>System should not cause or trigger any events that will leave Operating System in unrecoverable state</li>
</ul>
</li>
</ul>
<p><a></a></p>
<h1 id="testing-methodologies">5. Testing Methodologies</h1>
<hr>

    </div>
  </div>
</body>

</html>
