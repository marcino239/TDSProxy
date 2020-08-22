# TDSProxy

TDSProxy is a proxy server for the MS SQL Server TDS Protocol.

# sqls server connection monitor
[original code](https://github.com/tech-software/TDSProxy)


# Compile
```
choco install dotnet4.7.2
choco install netfx-4.7.2-devpack
choco install visualstudio2019buildtools
choco install nuget.commandline

cd TDSProxy\src
nuget restore
"c:\Program Files (x86)\Microsoft Visual Studio\2019\BuildTools\MSBuild\Current\Bin\amd64\MSBuild.exe" /property:Configuration=Release
```

# Run
- compile
- install certificate (menu: Cert, install: into Personal, password: "1")
- get certificate fingerprint and update config
- update server configuration in TDSProxy.exe.config
- bin/Release/TDSProxy.exe ShowSqlBatchText
- log in bin/Release/logs
