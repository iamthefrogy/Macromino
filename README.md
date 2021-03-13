<h1 align="center">
  <a href="https://github.com/iamthefrogy/frogy"><img src="https://user-images.githubusercontent.com/8291014/111030700-a4cf2180-83fb-11eb-840b-39185a478d85.png" alt="frogy" height=140px></a>
  </h1>
This repo is a knowledge-base/checklist. It consists of all the techniques of generating and supplying malicious macro-enabled excel files during your pentest/red-teaming project.<br/><br/>
    
**Attack techniques:-**
1. Excel presented with Fake DocuSign instructions to enable content.
2. Macros create temp folders in user folder and download a series of other files for the encoded PowerShell execution.
3. Macros create an hta file that contains implant download commands.
4. Basic evasion technique - Change file names frequently.
5. Macros can be crafted in password-protected 'sheets'.
6. Code can be obfuscated using the CHAR function within excel.
7. Auto-open functionality can be used with macro-enabled excel docs.
8. Pop-ups can be used in the spreadsheet to evade screenshot detection.
9. Checks can be written in macros to determine if the excel is opened in the sandbox or virtual environment or not.
10. Excel sheets can be hidden and also can be 'very hidden'. Hidden Sheets can be made visible either through the Excel GUI of the file, but Very Hidden Sheets cannot be unhidden through the Excel GUI. - https://www.ablebits.com/office-addins-blog/2017/12/20/very-hidden-sheets-excel/ 

**Warning/Disclaimer:** Read the detailed disclaimer at my blog - https://infosecninja.blogspot.com/p/blog-page.html</br>
Logo credit - www.designevo.com
