| Windows | Linux | OS X |
| :---- | :------ | :---- |
[![Windows build status][1]][2] | [![Linux build status][3]][4] | [![OS X build status][5]][6] | 

[1]: https://ci.appveyor.com/api/projects/status/j1evinfefeetctvk?svg=true
[2]: https://ci.appveyor.com/project/stratis/breeze
[3]: https://travis-ci.org/stratisproject/Breeze.svg?branch=master
[4]: https://travis-ci.org/stratisproject/Breeze
[5]: https://travis-ci.org/stratisproject/Breeze.svg?branch=master
[6]: https://travis-ci.org/stratisproject/Breeze


# Stratis Wallet (codename 'Storm')

__Warning: We're still in alpha, so use at your own risk.__
This is the repository of the Stratis Wallet, a full node staking wallet using Angular and Electron at the front-end and C# with .NET Core in the back-end.

## Daemon Build

The StratisD daemon is the backend REST service, hosting a Stratis node upon which FullNode UI depends:

```
# Clone and go in the directory
git clone https://github.com/stratisproject/FullNode.UI
cd FullNodeUI

# Initialize dependencies
git submodule update --init --recursive

# Run the StratisD daemon
cd StratisBitcoinFullNode/src/Stratis.StratisD
dotnet run -testnet
```

## UI Build

[Read more...](https://github.com/stratisproject/FullNodeUI/tree/master/FullNode.UI/README.md)

## CI Build
-----------

We use [AppVeyor](https://www.appveyor.com/) for Windows CI builds and [Travis CI](https://travis-ci.org/) for our Linux and MacOS ones.
Every time someone pushes to the master branch or create a pull request on it, a build is triggered and a new unstable app release is created.

To skip a build, for example if you've made very minor changes, include the text **[skip ci]** or **[ci skip]** in your commits' comment (with the squared brackets).

If you want the :sparkles: latest :sparkles: (unstable :bomb:) version of the wallet app, you can get it here: 

|    | x86 Release | x64 Release | Notes |
|:---|----------------:|------------------:|------------------:|
|**Windows**| [download][7] | [download][8] | Windows 7 and Windows 10 |
|**Linux**| - | [download][9] | All Linux flavors |
|**OS X**| - | [download][10] | OSX 10.12 or later |


[7]: https://github.com/stratisproject/Breeze/releases/download/cd-unstable/Breeze.Wallet-v0.3.0-setup-win-ia32.exe
[8]: https://github.com/stratisproject/Breeze/releases/download/cd-unstable/Breeze.Wallet-v0.3.0-setup-win-x64.exe
[9]: https://github.com/stratisproject/Breeze/releases/download/cd-unstable/Breeze.Wallet-v0.3.0-linux-x64.tar.gz
[10]: https://github.com/stratisproject/Breeze/releases/download/cd-unstable/Breeze.Wallet-v0.3.0-mac.dmg


