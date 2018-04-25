

#         Integrated scripting environment 


                Open PowerShell ISE
                
                $taure =  get-service -name webclient


                Write-Host "The service "$taure.name" is "$taure.status" "
                
                
                Try doing the Census example on ISE
                
 ##       Functions
 
                  
                Function Just-the-first
                {
                         param([int]$num1, [int]$num2)
                         $num1+$num2

                }
                Just-the-first -num1 123 -num2 243
                
                  
                  
                Function Just-the-first
                {
                          param([int]$num1, [int]$num2)
                          $num1+$num2

                }

                $result = Just-the-first -num1 123 -num2 243  


                  
      

                  
                  


          
