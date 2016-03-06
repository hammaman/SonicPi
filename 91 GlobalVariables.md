-------------------------------------------------------------------------------------------

  SONG COMPOSER V1
    Written by Andrew Hammacott
    For Sonic Pi by Sam Aaron

-------------------------------------------------------------------------------------------

  GLOBAL VARIABLES WHICH CHANGE
  In the order they appear
  
  $keynote     = (MIDI) value of the base note in the required key
                 for example, 72 = C6 or 60 = middle C (C5)

  $key5cale    = array of values to add to the base note value to get all the notes
                 in the required scale
			     Set this to either $major5cale or $minor5cale
			  
  $thissong    = array of values which represent the type of bar in the song
                 The type of bar can be one of the following:
			      1 .. Rest (i.e. nothing is playing)
                  2 .. Intro (opening few bars)
                  3 .. Verse 
                  4 .. Chorus
                  5 .. Bridge (this can be added as a link between to elements)
                  6 .. Chorus shifted up 5
                  7 .. End (i.e. ending few bars)
				
  $beatsinabar = number of beats in each bar   
  
  $beattime    = time between each beat in seconds

  $tunerythum  = array of values being the rythum of notes in the tune
                 The values can be:
			      0 which indicates no note is played for one beat
                  1 which indicates that a note will be played for one beat
                  2 which indicates that a note will be played for two beats
                    (unless there is only one beat left in the bar)
                 This is set up as a pattern of values which are randomly shuffled
				 
  $turnoffsnare  = flag to turn off the snare if set to 1
  $turnoffcymbal = flag to turn off the cymbal if set to 1
  $turnoffbass   = flag to turn off the base line if set to 1
  $turnofftriad  = flag to turn off the chords if set to 1
 
  

  
