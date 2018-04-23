#### GO TO *[HOME PAGE](index.md)*

#  Hash Tables

            
            
            
            PS C:\Users\pyelgoi> $employeNumbers = @{"prem" = 42433 ; "ram" = 3244325 ; "upender" = 32432432 ; "suraj" = 32432}
            PS C:\Users\pyelgoi> $employeNumbers

            Name                           Value
            ----                           -----
            suraj                          32432
            prem                           42433
            ram                            3244325
            upender                        32432432
            
            
            
            PS C:\Users\pyelgoi> $employeNumbers["ram"]
            3244325
            PS C:\Users\pyelgoi> $employeNumbers["ram"]= 435435435435435543554243
            PS C:\Users\pyelgoi> $employeNumbers

            Name                           Value
            ----                           -----
            suraj                          32432
            prem                           42433
            ram                            435435435435435543554243
            upender                        32432432


            PS C:\Users\pyelgoi> $employeNumbers["newname"]= 2343267
            PS C:\Users\pyelgoi> $employeNumbers

            Name                           Value
            ----                           -----
            suraj                          32432
            prem                           42433
            ram                            435435435435435543554243
            newname                        2343267
            upender                        32432432
            
            PS C:\Users\pyelgoi> $employeNumbers.remove("newname")
            PS C:\Users\pyelgoi> $employeNumbers

            Name                           Value
            ----                           -----
            suraj                          32432
            prem                           42433
            ram                            435435435435435543554243
            upender                        32432432


####  GO *[BACK](index.md)*



