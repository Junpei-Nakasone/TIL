

```javascript
 export function onOpen(): void {
  const spreadsheet = SpreadsheetApp.getActiveSpreadsheet();
  const menuEntries = [
      { name: 'menuEntryName', functionName: 'AddFunctionNameHere', },
  ];
  spreadsheet.addMenu('MenuNameHere', menuEntries);
}

```
