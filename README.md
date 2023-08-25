{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Debug with nodemon",
      "type": "node",
      "request": "launch",
      "runtimeExecutable": "nodemon",
      "runtimeArgs": ["-r", "ts-node/register"],
      "args": ["${workspaceFolder}/app/index.ts"],
      "cwd": "${workspaceFolder}",
      "console": "integratedTerminal",
      "internalConsoleOptions": "neverOpen",
      "restart": true,
      "protocol": "inspector",
      "outputCapture": "std",
      "sourceMaps": true,
      "skipFiles": ["<node_internals>/**"],
      "env": {
        "TS_NODE_PROJECT": "${workspaceFolder}/tsconfig.json"
      }
    }
  ]
}
