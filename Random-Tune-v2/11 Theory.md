-------------------------------------------------------------------------------------------

  SONG COMPOSER V2
    Written by Andrew Hammacott
    For Sonic Pi by Sam Aaron

-------------------------------------------------------------------------------------------

  THEORY
  
  1. CONSTRUCTING THE KEY SCALE
  
  Each octave is made up of 12 "notes" (half-steps or hs)
  (These are the natural notes such as F together with sharps/flats,
  so both the black and white keys on a piano)
  of which 7 are used in the particular key
  (for example, G major is made up of: G, A, B, C, D, E, F [and G])

  For the song, we need to specify the key
  this is made up of the MIDI key value, e.g. 72 = C5, 60 = C4, etc
  and whether the key is a major or minor 5cale
  
  The MIDI key values increase by 1 for each half-step, so an octave spans 12 successive values

  Mathematically, the major or minor scale can be constructed by adding
  a pattern of numbers to get all 7 notes in the scale.  The pattern is expressed
  as an addition to the previous (MIDI) note value: 
  base, +2hs, +2hs, +1hs, +2hs, +2hs, +2hs, +1hs     for a major scale
  base, +2hs, +1hs, +2hs, +2hs, +1hs, +2hs, +2hs     for a minor scale

