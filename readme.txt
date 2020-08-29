<<< This is a program that determines the mood of a playlist, album, or song from Spotify >>>

--To run--
	-create an app in spotify developer dashboard
	-use SET command in windows (export in mac) to set environemnt variable (client id, secret, and redirect URL)
	-Navigate to the directory of the main file and use command 'python spotify_mood.py "username"'
	-Then follow the prompts
		-If first time for the username it will ask you to enter the redirected url (after agreeing) into cmd. After the first
		time it will store it automatically.
		-the other prompts should be self explanatory

--How it works--
	-This is a very simplistic view of music moods and a I hope to implement more advanced music theory in the future.
	-There are four mood: Angry, Happy, Mellow, Sad
	-To determine these I used two metric spotify provides called energy and valence
		-Energy is self explanatory
		-Valence measures the positivity/negativity
		-Both run on a 0.0-1.0 scale
	-Angry = High energy, Low valence
	-happy = High energy, High valence
	-Mellow = low energy, high valence
	-Sad = low energy, Low valence