{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Debug index.ts",
      "type": "node",
      "request": "launch",
      "program": "${workspaceFolder}/app/index.ts",
      "cwd": "${workspaceFolder}/app",
      "preLaunchTask": "CleanAndBuild"
    }
  ],
  "tasks": [
    {
      "label": "CleanAndBuild",
      "type": "shell",
      "command": "rm -rf dist && npm run build",
      "group": {
        "kind": "build",
        "isDefault": true
      }
    }
  ]
}
