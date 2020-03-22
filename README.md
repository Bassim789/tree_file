# Filedir
Filedir is a simple tool that can scan files and folders inside a given path.
The data produced by the scan are portable and can be visualized in a browser.

Demo: [http://www.filedir.ch/demo](http://www.filedir.ch/demo)

## Scanning
Download the repo and place it on your computer or a server you want to scan.
It needs to be linux or mac and to have python 2 or 3 installed, most computer and server have it by default.

### Automatic
For the first time you run the app, right click on the scan.command file and select "open with" and "Terminal.app", then click ok to accept to run this app. For the next time you just have to double click on scan.command file.
By default your home folder will be scanned, if it takes too much time or you want to scan another folder, just edit the scan.command file and put the path you want after "python scan.py" insteed of the ~ symbol.

### Manual
Open a terminal and go to the repo.

Then use the following command:
```
python scan.py path/you/want/to/scan
```
If an error with encoding appear, you can try adding "latin1" as an argument at the end of the command.

After the scan, the file data.json.js is created inside the repo, it contains the result of the scan.

## Visualization
If necessary, move or copie the repo on a location where you can see html files.
Inside the repo open the index.html file on a modern browser like Chrome or Firefox (Internet explorer not supported).
Here you can see your files and folders.
- Click on a folder to see what's inside or click on the folder of the path to go back.
- Click on a file type to restrain the view to only this type of file, click again to deselect it.
- Activate the dark mode by clicking on the top right button.

## Folder description
You can add a special file inside folders that will be used as a description for the folder.
They have to be named like this
```
_info.txt
```

## Future development
- Add file description with .info.txt files.
- Support windows scanning (currently only mac and linux)
- Change the way the data are loaded inside the browser to scale better (for now you can reach about half a million files).
- Add test for the scanning and the visualization.

## License
This tool is on GPL3 license.
