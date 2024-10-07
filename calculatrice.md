PS C:\> Set-Location c:\
Get-Process | Where-Object {$_.Name -like "calc*"}

Handles  NPM(K)    PM(K)      WS(K)     CPU(s)     Id  SI ProcessName              
-------  ------    -----      -----     ------     --  -- -----------              
    612      44    29832      83024       1,13  10624  10 CalculatorApp            
    454      36    16236       5716       0,47  12456  10 CalculatorApp            
    609      44    29492      82556       0,95  12852  10 CalculatorApp            



PS C:\> Get-History

  Id CommandLine                                                                   
  -- -----------                                                                   
   1 Get-Host                                                                      
   2 Get-Host | Select-Object -Property Version                                    
   3 (Get-Host).GetType()                                                          
   4 (Get-Host | Select-Object -Property Version).GetType()                        
   5 (Get-Host | Select-Object -Property Version).Version                          
   6 $ObjVersion = (Get-Host | Select-Object -Property Version).Version...         
   7 $ObjVersion = (Get-Host | Select-Object -Property Version).Version...         
   8 $ObjVersionMajor                                                              
   9 Start-Process calc.exe...                                                     
  10 Set-Location c:\...                                                           
  11 Set-Location c:\...            
