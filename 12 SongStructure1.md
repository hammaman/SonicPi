-------------------------------------------------------------------------------------------

  SONG COMPOSER V1
    Written by Andrew Hammacott
    For Sonic Pi by Sam Aaron

-------------------------------------------------------------------------------------------

  SONG STRUCTURE (PART 1)

  I have attempted to develop a song with a structure made up of the following elements
  
  1 .. Rest (i.e. nothing is playing)
  2 .. Intro (opening few bars)
  3 .. Verse 
  4 .. Chorus
  5 .. Bridge (this can be added as a link between to elements)
  6 .. Chorus shifted up 5
  7 .. End (i.e. ending few bars)

  A song can be made up of an array of bars (specified as a ring), where each bar is
  specified as a certain type, denoted by a number between 1 and 7 according to the
  list above
  
  For example, I have determined for this song, the rest is one bar, the intro goes on for 3 bars,
  and so on ...
  thissongrest = (ring 1)                 #just one bar
  thissongintro = (ring 2,2,2)            #made up of three bars
  thissongverse = (ring 3,3,3,3,3,3,3,3)  #made up of 8 bars
  thissongchorus = (ring 4,4,4,4)         #made up of 4 bars
  thissongbridge = (ring 5,5,5)           #made up of 3 bars
  thissonglastchorus = ring(6,6,6,6)      #made up of 4 bars
  thissongend = ring(7,7,7,7,7,7)         #made up of 6 bars

  We then add these together to give the structure of the song
  This is stored in the global variable $thissong