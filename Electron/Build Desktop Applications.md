
## Offcal Document
https://www.electron.build/

## Pre-Install
```- npm install -g asar```  

```- npm install electron-builder --dev```

## Configuration

- ### package.json  
```
  "scripts": {
    "start": "electron .",
    "dist": "build"
  }
  "build": {
  	"productName": "${name}",
    "copyright": "",

    "appId": "com.electron.${name}",
    "artifactName": "${productName}-${version}.${ext},
	"asar": "true",

    "win": {
      "target": "nsis",
      "icon": "dist/icons/icon.ico"
    },
    "mac": {
      "target": "zip",
      "icon": "dist/icons/icon.icns"
    }
  }

```