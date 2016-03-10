-------------------------------------------------------------------------------------------

  SONG COMPOSER V2
    Written by Andrew Hammacott
    For Sonic Pi by Sam Aaron

-------------------------------------------------------------------------------------------

  SONG STRUCTURE (PART 2)

  Next, we determine how many beats are in the bar
  
  I have defined a beat to be the equivalent to a half-note
  and so the song contains no notes which are quicker than half-notes
  This means that the number of beats in the bar and the time between each beat
  when combined give a more usual time signature

  An example is:  
  $beatsinabar = 8   Number of beats in each bar
  $beattime = 0.25   Time between each beat in seconds
  
  You will see that there are 4 beats per second, so 240 beats per minute.  This may sound
  fast, but the intention is not to have a drum beat on every beat, but instead on every
  other beat, so giving a more reasonable 120 bpm
