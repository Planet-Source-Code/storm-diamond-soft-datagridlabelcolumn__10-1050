<div align="center">

## DataGridLabelColumn


</div>

### Description

A label style datagrid column is achived by inheriting the DataGridTextBoxColumn.

a good example of the simplicity and power of inheritance.
 
### More Info
 
A very basic example of inheritance.

this not the best way to do this. the best way is to inherit DataGridColumn directly but this is the easiest and the fastest way for achieving this.


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Storm \(Diamond Soft\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/storm-diamond-soft.md)
**Level**          |Beginner
**User Rating**    |4.3 (17 globes from 4 users)
**Compatibility**  |VB\.NET
**Category**       |[Controls/ Forms/ Dialogs/ Menus](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/controls-forms-dialogs-menus__10-3.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/storm-diamond-soft-datagridlabelcolumn__10-1050/archive/master.zip)

### API Declarations

Use it as you will


### Source Code

```
Public Class DataGridLabelColumn
  Inherits DataGridTextBoxColumn
  'Just overrides the base edit methods
  'This way no edit is done at all and the column behaves as a label
  '
  Protected Overloads Overrides Sub Edit(ByVal source As System.Windows.Forms.CurrencyManager, ByVal rowNum As Integer, ByVal bounds As System.Drawing.Rectangle, ByVal [readOnly] As Boolean, ByVal instantText As String)
  End Sub
  Protected Overloads Overrides Sub Edit(ByVal source As System.Windows.Forms.CurrencyManager, ByVal rowNum As Integer, ByVal bounds As System.Drawing.Rectangle, ByVal [readOnly] As Boolean, ByVal instantText As String, ByVal cellIsVisible As Boolean)
  End Sub
  Protected Overloads Overrides Sub Edit(ByVal source As System.Windows.Forms.CurrencyManager, ByVal rowNum As Integer, ByVal bounds As System.Drawing.Rectangle, ByVal [readOnly] As Boolean)
  End Sub
End Class
```

