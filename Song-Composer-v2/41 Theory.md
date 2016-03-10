-------------------------------------------------------------------------------------------

  SONG COMPOSER V2
    Written by Andrew Hammacott
    For Sonic Pi by Sam Aaron

-------------------------------------------------------------------------------------------

  THEORY
  
  2. CONSTRUCTING TRIADS FOR EACH NOTE IN THE KEY

     Each note in the 5cale (there are 7) has a triad of three notes associated with it.
     I've given an example of each note in the 5cale of C major
     1st note (e.g. C) .. major triad
     2nd note (e.g. D) .. minor triad
     3rd note (e.g. E) .. minor triad
     4th note (e.g. F) .. major triad
     5th note (e.g. G) .. major triad
     6th note (e.g. A) .. minor triad
     7th note (e.g. B) .. minor triad

    In summary
    If triad is based on 1st, 4th or 5th note in the octave of the chosen scale .. major
    Otherwise if based on 2nd, 3rd, 6th or 7th .. minor

  3. MAKING SOUNDS FROM A PROGRESSION OF TRIADS
  
     A nice sounding sequence of triads can be expressed mathematically
     by a set of rules.  The rules are expressed in this way below.
	 
	 1st triad can be followed by any triad
	 2nd triad can be followed by 1st, 5th or 7th triads
	 3rd triad can be followed by 1st, 2nd, 4th or 6th triads
	 4th triad can be followed by 1st, 2nd, 3rd, 5th or 7th triad
	 5th triad can be followed by 1st or 6th triad
	 6th triad can be followed by 1st, 2nd, 3rd, 4th or 5th triad
	 7th triad can be followed by 1st or 3rd triad
	 
	 This can be programmed as an array for each triad, as follows
      $nextch1 = (ring 2,3,4,5,6,7)
      $nextch2 = (ring 1,5,7)
      $nextch3 = (ring 1,2,4,6)
      $nextch4 = (ring 1,2,3,5,7)
      $nextch5 = (ring 1,6)
      $nextch6 = (ring 1,2,3,4,5)
      $nextch7 = (ring 1,3)
