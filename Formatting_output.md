#### GO TO *[HOME PAGE](index.md)*

#   Formatting Output

        
        
        dir | Format-wide
        dir | Format-wide -Property length
        dir  | Format-list
        dir  | Format-list -property name , length , LastAccessTime
        dir  | Format-Table
        Get-Process | format-table
        Get-Process | format-table  name , ID , path , company
        Get-Process | format-table  name , ID , path , company -AutoSize
        Get-Process | format-table  name , ID , path , company -AutoSize -GroupBy company
        Get-Process |sort  -property company | format-table -property name,id,path -groupby company
        
        
####  GO *[BACK](index.md)*        
