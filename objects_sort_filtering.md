#### GO TO *[HOME PAGE](index.md)*


##  Objects

        
          PS C:\Users\pyelgoi> $file = dir
          PS C:\Users\pyelgoi> $file
          PS C:\Users\pyelgoi> $file | get-member
          PS C:\Users\pyelgoi> $file[0]  - gives 1st dir
          PS C:\Users\pyelgoi> $file[1]  - gives 2nd dir
          PS C:\Users\pyelgoi> $file[1] | get-member 
          (you can use the options when you do get-member, length etc,.)
          
          
##  Sort 
          
          
           PS C:\Users\pyelgoi> dir | sort -property -size -Desc
           help sort -online
           
##  Filtering

                
           help where -online
           PS C:\Users\pyelgoi> dir | where length -gt 500
           
           PS C:\Users\pyelgoi> dir | where name -like "*uper*"


           Directory: C:\Users\pyelgoi


          Mode                LastWriteTime         Length Name
          ----                -------------         ------ ----
         -a----        1/18/2018   1:45 PM           3439 SuperPuTTY.settings 
           
          dir | where {$_.length -gt 5000} 
          (current object "$_" ".property")
          
          dir | where {($_.length -gt 5000) -and ($_.Name -like "*B*")}
          
          PS C:\Users\pyelgoi> dir | where {($_.length -gt 500) -and ($_.name -like "*p*")}


          Directory: C:\Users\pyelgoi


          Mode                LastWriteTime         Length Name
          ----                -------------         ------ ----
         -a----        1/18/2018   1:45 PM           3439 SuperPuTTY.settings
          
          
####  GO *[BACK](index.md)*          
          
           
          
          
