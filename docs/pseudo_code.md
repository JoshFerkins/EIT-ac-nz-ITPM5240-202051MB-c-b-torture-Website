---
theme: jekyll-theme-cayman
title: C&B Music Website
---

<h1>Pseudo</h1>

<a href="https://JoshFerkins.github.io/EIT-ac-nz-ITPM5240-202051MB-c-b-torture-Website/">Home</a>
Pseudocode:

BEGIN
	OPEN Application
	Call addUser() Module
	
	Select users who recently registered or logged in
	//All setting with respect to user will be restored like play Queue, user info etc
	Display Home Screen
	
	//Home screen has multiple options/functionality. Choose anyone.
	WHILE True DO
		IF option == "Play/Pause/Skip" THEN
			Call playPauseSkip() Module
                ELSE IF option == "Add Playlist" THEN
                        Call addPlaylist() Module
                ELSE IF option == "Add Song" THEN
                        Call addSong() Module
		ELSE IF option == "Select Playlist" THEN
			Call selectPlayList() Module
		ELSE IF option == "Select Song" THEN
			Call selectSong() Module
		ELSE IF option == "Settings" THEN
			Call settings() Module
		ELSE IF option == "Logout" THEN
			EXIT
		END IF
	END WHILE
END

BEGIN addUser
	//Input information about user
	INPUT name, email, userName, phoneNo, password
	Confirm on the details entered
	
	Create user based on input details
END addUser

BEGIN playPauseSkip
	//When user logs in, play Queue is retrieved based on user choice earlier or is empty for new user
	Select a song that you wish to play.
	Add song to play Queue
	Play the song from Queue.
	
	Play/Pause button to play or pause the song.
	Left button to play previous song.
	Right button to play next song.
END playPauseSkip

BEGIN selectPlayList
	Left Panel has a list of Playlists and Create PlayList Option.
	Select the Playlist of your choice
	Songs from the selected PlayList will be added to play Queue
END selectPlayList

BEGIN addPlaylist
        Select Create Playlist
        SELECT Mofu
        INPUT playlistName
        Empty playlist created with "playlistName"
END addPlaylist

BEGIN addSong
        Select Add Song
        Call addSong() module
        Select Playlist
        Add song to Playlist
END addSong

BEGIN selectSong
	Select Songs displayed on Home Page or from PlayList
	Song will be played immediately
END selectSong

BEGIN settings
	Select drop-down on the Top header right side of Logo.
	Choose Settings from the Drop-down.
	
	Display Available options in settings
	Colour Theme
	Light/Dark Mode
	Volume Mixer
	Move Elements
	Manage Users
	View FAQs
	Support
END settings
