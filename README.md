<div align="center">

## Project File Name Correction


</div>

### Description

Eliminate short name conversion in the VB IDE.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[James E\. Toebes](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/james-e-toebes.md)
**Level**          |Beginner
**User Rating**    |5.0 (10 globes from 2 users)
**Compatibility**  |VB 5\.0, VB 6\.0
**Category**       |[VB function enhancement](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/vb-function-enhancement__1-25.md)
**World**          |[Visual Basic](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/visual-basic.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/james-e-toebes-project-file-name-correction__1-8777/archive/master.zip)





### Source Code

```
Ever noticed that if you open a vb project containing a long file name from explorer by double clicking it shortens the filename to 'PROJEC~1' instead of 'Project Number 1'? But if you open the same project while inside VB (Project open dialog) it uses the long name.
I experimented and found a quick fix.
1. From Explorer choose View => Folder Options
2. Select the tab 'File Types'
3. Scroll through the list and highlight 'Visual Basic Project' then press the Edit button.
4. Highlight 'Open' then press the Edit button.
5. Change the 'Application used to preform this action
 from C:\Program Files\DevStudio\VB\vb5.exe "%1"
 to "C:\Program Files\DevStudio\VB\vb5.exe" "%1"
 NOTE: the only change is adding double quotes around the VB5.exe specification.
6. Save the changes.
You can repeat this for the other items in both the actions list and the registered applications list.
If any one can give me a reasonable explanation as to why this works, I would sure appreciate it. Interesting that if you try to make changes without adding the quotes, Your told that it is invalid and cannot save it.
```

