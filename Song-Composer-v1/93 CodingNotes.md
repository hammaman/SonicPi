-------------------------------------------------------------------------------------------

  SONG COMPOSER V1
    Written by Andrew Hammacott
    For Sonic Pi by Sam Aaron

-------------------------------------------------------------------------------------------

 NOTES ON THE CODE USED

 I've broken a key rule with live loops by not including a sleep command
  As we are syncing each subsequent live loop, this means that the loop will wait
  until it is in sync with the timing loop and so I don't need a sleep command

 Sonic Pi gets very upset if you use any keywords
  so I've had to "misspell" the words ch0rd and 5cale when writing my comments

 You will also see many variables which start with $ - these are global variables
  which can be used across the live loops

 I am also using arrays which let me store multiple values using one variable name
  for example, major5cale[]
  The number in the bracket is the index to which value I need
  and the first value is stored in index 0, the second in index 1, and so on

 I have also converted numbers to text to be able to print out messages
  using the Ruby .to_s suffix
