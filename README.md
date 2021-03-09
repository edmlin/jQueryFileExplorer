# jQueryFileExplorer
Inspired by [jQueryFiletree](https://github.com/jqueryfiletree/jqueryfiletree). Most of the icons in the images folder are from [jQueryFiletree](https://github.com/jqueryfiletree/jqueryfiletree/tree/master/dist/images).
## Usage
```
$(selector).jQueryFileExplorer({
	root: "/",
	rootLabel: "Server",
	script: "https://localhost:44316/FileExplorer/GetPath",
	fileScript: "https://localhost:44316/FileExplorer/GetPath"
});)
```
## Parameters:
 - root: the path of the root passed to the backend url or function
- rootLabel: the label of the root shown in the file explorer
- script: the URL or a function that responds with folder information.
- fileScript: a function or a URL to download the file when a file is clicked
### Note:
If the script/fileScript is a function, an object parameter {path: 'path'} is passed to the function. If the script/fileScript is a URL, a parameter 'path' with the path of the clicked folder/file is passed to the URL via POST(for folders) or GET(for files).
## Screenshot
![Screenshot](https://github.com/edmlin/jQueryFileExplorer/raw/master/Demo.jpg)
