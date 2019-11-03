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

# Build bundle

```
# Only android bundle
npm run bundle-android

# Only ios bundle
npm run bundle-ios

# Only androdi + ios bundle
npm run bundle
```

# COnfig TeamCity

## Step NPM install

```
echo ‘ ---------->Step NPM install’
pwd

echo 'check npm,start'
# npm get config get proxy
# npm get config get https-proxy
npm get config get respository
echo 'check npm,end'

# npm get config set proxy
# npm get config set https-proxy
npm get config set respository http://registry.npm.taobao.org/

echo 'check npm,start'
# npm get config get proxy
# npm get config get https-proxy
npm get config get respository
echo 'check npm,end'

echo ‘<----------Step NPM install’
```
