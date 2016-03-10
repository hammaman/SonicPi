-------------------------------------------------------------------------------------------

  SONG COMPOSER V2
    Written by Andrew Hammacott
    For Sonic Pi by Sam Aaron

-------------------------------------------------------------------------------------------

  SETTING THE SONG UP

  The user needs to make the following decisions

  - Choosing a random seed to use
  
      This is done by setting the seed in the use_random_seed line
   
   - Choosing a key for the song to be in
   
      This is done by setting the values of:
	    $keynote = MIDI value of the starting note in the scale
		$key5cale = $major5cale or $minor5cale, depending on whether major or minor

  NOTE: the song can only in one key (there is only one at the moment)

