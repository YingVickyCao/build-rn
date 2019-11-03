# Run jest tests

```
npm run jest-test
npm run jest-test-coverage
```

# Run tests in VsCode

https://jestjs.io/docs/en/troubleshooting#debugging-in-vs-code

```
{
  "version": "0.2.0",
  "configurations": [
    {
      "name": "Debug Jest Tests",
      "type": "node",
      "request": "launch",
      "runtimeArgs": [
        "--inspect-brk",
        "${workspaceRoot}/node_modules/.bin/jest",
        "--runInBand"
      ],
      "console": "integratedTerminal",
      "internalConsoleOptions": "neverOpen",
      "port": 9229
    }
  ]
}
```
