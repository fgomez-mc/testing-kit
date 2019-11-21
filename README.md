## Testing Training

To get started with the project cd into the location and `npm i`.

Topics that we will cover:

- Forking

- toJson & Enzyme

- $r

- React dev to

- Redux dev tools

- Break points

- repl.it

- Prettier

`launch.json`

```javascript
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Debug CRA Tests",
            "type": "node",
            "request": "launch",
            "runtimeExecutable": "${workspaceRoot}/node_modules/.bin/react-scripts",
            "args": ["test", "--runInBand", "--no-cache", "--watchAll=false"],
            "cwd": "${workspaceRoot}",
            "protocol": "inspector",
            "console": "integratedTerminal",
            "internalConsoleOptions": "neverOpen",
            "env": { "CI": "true" },
            "disableOptimisticBPs": true
        }, 
        {
            "type": "chrome",
            "request": "launch",
            "name": "Launch Chrome",
            "url": "http://localhost:3000",
            "webRoot": "${workspaceFolder}"
        }
    ]
}
```
