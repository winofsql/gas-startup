# gas-startup

![image](https://user-images.githubusercontent.com/1501327/189235965-e95dfdb9-af66-4f19-ba33-103e6d59a402.png)

- ## [Google Apps Script 正式ドキュメント](https://developers.google.com/apps-script/reference)
  - ## [Class SpreadsheetApp](https://developers.google.com/apps-script/reference/spreadsheet/spreadsheet-app)
  - ## [Class Ui](https://developers.google.com/apps-script/reference/base/ui)
    ![image](https://user-images.githubusercontent.com/1501327/189239087-5c5ac73e-7408-4e7d-89a6-05f4f34c8e33.png)
    ![image](https://user-images.githubusercontent.com/1501327/189239151-3a73769d-96a3-484b-99a4-ab5a527ee4db.png)
    
```javascript
function myFunction() {

  var ss = SpreadsheetApp.getActiveSpreadsheet();
  var sheet = ss.getSheets()[0];
  Logger.log(sheet.getName());
  // Logger.log(ss.getUrl());

  SpreadsheetApp.getUi().alert('Hello, world');

}
```

```javascript
function test() {

  var spreadsheet = SpreadsheetApp.getActive();
  spreadsheet.getRange('A1').activate();
  spreadsheet.getCurrentCell().setValue('1');
  spreadsheet.getActiveRange().autoFill(spreadsheet.getRange('A1:A16'), SpreadsheetApp.AutoFillSeries.ALTERNATE_SERIES);

}
```
