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
				
  $beatsinabar = number of beats in each bar   
  
  $beattime    = time between each beat in seconds
