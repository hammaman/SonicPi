-------------------------------------------------------------------------------------------

  SONG COMPOSER V2
    Written by Andrew Hammacott
    For Sonic Pi by Sam Aaron

-------------------------------------------------------------------------------------------

  SONG STRUCTURE (PART 3)

  Next, we define a rythum for the tune.

  In the last part, we defined the number of beats in the bar and now need to work out
  on which beats a note in the tune will be played.
  
  This is done by randomly shuffling the global $tunerythum ring which contains
    0 which indicates no note is played for one beat
    1 which indicates that a note will be played for one beat
    2 which indicates that a note will be played for two beats
      (unless there is only one beat left in the bar)

