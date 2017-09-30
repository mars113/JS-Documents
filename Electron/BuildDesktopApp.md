
## 官方文件
https://www.electron.build/

.

## 發佈前準備

- 安裝 asar 套件  
```- npm install asar -g```  


- 安裝 electron-build 套件  
```- npm install electron-builder -D```

.

## Configuration

- ### package.json  
```
  "scripts": {
    "start": "electron .",
    "dist": "build"
  },
  
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

.


## 建置專案
```npm run dist```