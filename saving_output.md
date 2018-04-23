#### GO TO *[HOME PAGE](index.md)*

# Saving Output


       get-process | Out-File c:output.txt
       notepad  C:\Users\pyelgoi\output.txt
       PS C:\Users\pyelgoi> notepad  C:\Users\pyelgoi\output.txt
       PS C:\Users\pyelgoi> get-process | Out-File c:output.txt
       PS C:\Users\pyelgoi> Get-Process | ConvertTo-Html | Out-File C:output1.txt
       PS C:\Users\pyelgoi> Invoke-Expression C:\Users\pyelgoi\output1.txt
       PS C:\Users\pyelgoi> notepad  C:\Users\pyelgoi\output.txt
       PS C:\Users\pyelgoi> get-process | Out-File c:output.txt
       PS C:\Users\pyelgoi> Get-Process | ConvertTo-Html | Out-File C:output1.txt
       PS C:\Users\pyelgoi> Invoke-Expression C:\Users\pyelgoi\output1.txt
       PS C:\Users\pyelgoi> Get-Process | Export-Csv c:output2.csv
       PS C:\Users\pyelgoi> Invoke-Expression C:\Users\pyelgoi\output2.csv
       PS C:\Users\pyelgoi>
       
####  GO *[BACK](index.md)*
  
  
  
