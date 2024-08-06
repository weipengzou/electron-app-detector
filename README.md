# electron-app-detector

## MAC
```cmd
find /Applications -type d -path '*/Contents/Frameworks/Electron Framework.framework' -exec dirname {} \; | xargs -I {} dirname {} | xargs -I {} echo {} | uniq
```


## Result
```cmd
/Applications/Microsoft Teams classic.app/Contents
/Applications/Visual Studio Code.app/Contents
/Applications/Figma.app/Contents
/Applications/Notion.app/Contents
/Applications/Docker.app/Contents/MacOS/Docker Desktop.app/Contents
```
