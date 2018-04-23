 #### GO TO *[HOME PAGE](index.md)*
 
 #  Manipulate Data
 
      Use Census1000.csv file for practice
      
      $names = Import-Csv C:\Users\pyelgoi\Desktop\Census1000.csv
      $names | Get-Member
      
      
      Mostly used surname in hispanic community 
      
      $names | sort -Property pcthispanic | Format-Table -Property name, pcthispanic
      
      
       PS C:\Users\pyelgoi> ($names | sort -Property pcthispanic -descending)[0]


      name         : BARAJAS
      rank         : 989
      count        : 32147
      prop100k     : 11.92
      cum_prop100k : 40439.43
      pctwhite     : 3.28
      pctblack     : 0.17
      pctapi       : 0.17
      pctaian      : 0.18
      pct2prace    : 0.23
      pcthispanic  : 95.97

      PS C:\Users\pyelgoi> ($names | sort -Property pcthispanic -descending)[0].name
      BARAJAS
      
      PS C:\Users\pyelgoi> $names | sort -Property pcthispanic -descending| select -First 1


      name         : BARAJAS
      rank         : 989
      count        : 32147
      prop100k     : 11.92
      cum_prop100k : 40439.43
      pctwhite     : 3.28
      pctblack     : 0.17
      pctapi       : 0.17
      pctaian      : 0.18
      pct2prace    : 0.23
      pcthispanic  : 95.97


      PS C:\Users\pyelgoi> $names | sort -Property pcthispanic -descending| select -First 10
      
      PS C:\Users\pyelgoi> $names | sort -Property pcthispanic -descending| select -First 10 | Format-Table -Property name

      name
      ----
      BARAJAS
      ZAVALA
      OROZCO
      VELAZQUEZ
      MEZA
      JUAREZ
      IBARRA
      HUERTA
      VAZQUEZ
      CERVANTES
      
      
####  GO *[BACK](index.md)*      


      
      
      
      
      
      
      
      
      
