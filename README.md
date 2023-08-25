{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Debug index.ts",
      "type": "node",
      "request": "launch",
      "program": "${workspaceFolder}/index.ts",
      "cwd": "${workspaceFolder}",
      "protocol": "inspector",
      "runtimeArgs": ["--nolazy", "-r", "ts-node/register"],
      "internalConsoleOptions": "openOnSessionStart",
      "sourceMaps": true,
      "outFiles": ["${workspaceFolder}/dist/**/*.js"]
    }
  ]
}
