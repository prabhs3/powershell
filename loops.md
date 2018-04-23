#### GO TO *[HOME PAGE](index.md)*

#Loops


      PS C:\Users\pyelgoi> 1..10
      1
      2
      3
      4
      5
      6
      7
      8
      9
      10
      PS C:\Users\pyelgoi>
      
      
      PS C:\Users\pyelgoi> 1..10 | foreach{$_*2}
      2
      4
      6
      8
      10
      12
      14
      16
      18
      20
      PS C:\Users\pyelgoi>
    
      PS C:\Users\pyelgoi> 1..10 | foreach {"This is the loop number $_"}
      This is the loop number 1
      This is the loop number 2
      This is the loop number 3
      This is the loop number 4
      This is the loop number 5
      This is the loop number 6
      This is the loop number 7
      This is the loop number 8
      This is the loop number 9
      This is the loop number 10
      PS C:\Users\pyelgoi>

      PS C:\Users\pyelgoi> 1..10 | foreach{"*"*$_}
      *
      **
      ***
      ****
      *****
      ******
      *******
      ********
      *********
      **********
      PS C:\Users\pyelgoi>
      
      PS C:\Users\pyelgoi> 1..10 | foreach {if($_%2){"$_ is odd"}}
      1 is odd
      3 is odd
      5 is odd
      7 is odd
      9 is odd
      PS C:\Users\pyelgoi>


####  GO *[BACK](index.md)*
