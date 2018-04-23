#  Arrays


      PS C:\Users\pyelgoi> $strcomputer = @("ser1" , "ser2" , "ser3")
      PS C:\Users\pyelgoi> $strcomputer
      ser1
      ser2
      ser3
      PS C:\Users\pyelgoi> $strcomputer[0]
      ser1
      PS C:\Users\pyelgoi> $strcomputer[1]
      ser2
      PS C:\Users\pyelgoi> $strcomputer.length
      3
      PS C:\Users\pyelgoi> $strcomputer2 = @("ser5" , "ser6")
      PS C:\Users\pyelgoi> $strcomputer2
      ser5
      ser6
      PS C:\Users\pyelgoi> $allcomputers = $strcomputer + $strcomputer2
      PS C:\Users\pyelgoi> $allcomputers
      ser1
      ser2
      ser3
      ser5
      ser6
      PS C:\Users\pyelgoi> $allcomputers | foreach{$_.length}
      4
      4
      4
      4
      4
      PS C:\Users\pyelgoi> $allcomputers[4] = "pre"
      PS C:\Users\pyelgoi> $allcomputers | foreach{$_.length}
      4
      4
      4
      4
      3
      PS C:\Users\pyelgoi>
      
      PS C:\Users\pyelgoi> $allcomputers | foreach{$_ + "-" + $_.length}
      ser1-4
      ser2-4
      ser3-4
      ser5-4
      pre-3
      PS C:\Users\pyelgoi>

      
      
      
