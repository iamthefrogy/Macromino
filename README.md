<h1 align="center">
  <a href="https://github.com/iamthefrogy/frogy"><img src="https://user-images.githubusercontent.com/8291014/111030700-a4cf2180-83fb-11eb-840b-39185a478d85.png" alt="frogy" height=140px></a>
  </h1>
This repo is a knowledge-base/checklist. It consists of all the techniques of generating and supplying malicious macro-enabled excel files during your pentest/red-teaming project.<br/><br/>
    
![](https://visitor-badge.glitch.me/badge?page_id=iamthefrogy.Marcomino)<a href="https://twitter.com/iamthefrogy"> </a></br>     
##### Attack techniques
1. Excel presented with Fake DocuSign instructions to enable content.
2. Macros create temp folders in user folder and download a series of other files for the encoded PowerShell execution.
3. Macros create an hta file that contains implant download commands.
4. Macros run base64 encoded commands to download first and second stage backdoors to implant.
5. Basic evasion technique - Change file names frequently.
6. Macros can be crafted in password-protected 'sheets'.
7. Code can be obfuscated using the CHAR function within excel.
8. Auto-open functionality can be used with macro-enabled excel docs.
9. Macro with ana bility to create a scheduled task, both commonly known auto-start extensibility points (ASEPs).
10. Pop-ups can be used in the spreadsheet to evade screenshot detection.
11. Checks can be written in macros to determine if the excel is opened in the sandbox or virtual environment or not.- https://malware.news/t/excel-4-macros-get-workspace-reference/38892 . GET.WORKSPACE(int) can be used to perform various checks. Example:
GET.WORKSPACE(19) - checks for the presence of a mouse
GET.WORKSPACE(42) - checks if the device can play sounds
10. Excel sheets can be hidden and also can be 'very hidden'. Hidden Sheets can be made visible either through the Excel GUI of the file, but Very Hidden Sheets cannot be unhidden through the Excel GUI. - https://www.ablebits.com/office-addins-blog/2017/12/20/very-hidden-sheets-excel/<br/><br/>

##### Defence techniques
1. Use AMSI (Anti-malware scan interface) to block runtime execution of macro based documents. Ensure this feature should be enabled for all locations and not just trusted locations. - https://www.microsoft.com/security/blog/2021/03/03/xlm-amsi-new-runtime-defense-against-excel-4-0-macro-malware/
2. Disallow all legacy workbooks that require excel 4.0 and below.
3. Prevent internet originated macros.
4. Disallow macros or allow only macros from trusted locations.
5. Educate users on not enabling macros by clicking on enable content on any unexpected excel workbooks.
6. Use attack surface reduction rules to prevent users against Macro based phishing attacks. - https://docs.microsoft.com/en-us/microsoft-365/security/defender-endpoint/attack-surface-reduction?view=o365-worldwide

Warning/Disclaimer: Read the detailed disclaimer at my blog - https://github.com/iamthefrogy/Disclaimer-Warning/blob/main/README.md <br/>
Logo credit - www.designevo.com
