# Javascript


### Save File
```
const str  = 'test';
const blob = new Blob([str], {type: 'text/plain'});

// Create a link element to trigger the download
const lnk = document.createElement('a');
lnk.href = URL.createObjectURL(blob);
lnk.download = `file.txt`;
lnk.click();

// Clean up blob
URL.revokeObjectURL(lnk.href);
```