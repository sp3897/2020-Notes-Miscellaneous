## Use this config file to setup debug on your vs code

I know that its but do not want to google it everytime
Note : when you want to debug you need to be on the same file to start debugging on the VS Code editor

```
{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
      
        {
            "type": "node",
            "request": "launch",
            "name": "Launch Program",
            "program": "${workspaceFolder}/src/main/javascript/index.js"
        },
        {
           "name": "Debug spec.js",
           "type": "node",
           "request": "launch",
           "program": "${workspaceFolder}/node_modules/jasmine/bin/jasmine.js",
           "args": [
             "${file}"
           ], 
           "env": { 
             "NODE_PATH": "." 
           }
         }
    ]
}

