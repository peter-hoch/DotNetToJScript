# DotNet2JScript

## cmd line arguments

```powershell
.\DotNetToJScript\bin\x64\Release\DotNetToJScript.exe
Usage: DotNetToJScript v1.0.4 [options] path\to\asm
Copyright (C) James Forshaw 2017. Licensed under GPLv3.
Source code at https://github.com/tyranid/DotNetToJScript
Options
  -n                         Build a script which only uses mscorlib.
  -m                         Build a scriptlet file in moniker format.
  -u                         Build a scriptlet file in uninstall format.
  -d                         Enable debug output from script
  -l, --lang=VALUE           Specify script language to use (JScript, VBA,
                               VBScript)
  -v, --ver=VALUE            Specify .NET version to use (None, v2, v4, Auto)
  -o=VALUE                   Specify output file (default is stdout).
  -c=VALUE                   Specify entry class name (default TestClass)
  -s=VALUE                   Specify file with additional script. 'o' is
                               created instance.
      --clsid=VALUE          Specify a CLSID for the scriptlet
  -h, --help                 Show this message and exit
```

example cmd

```powershell
.\DotNetToJScript\bin\x64\Release\DotNetToJScript.exe .\StartCalculator\bin\x64\Release\StartCalculator.dll  --lang=Jscript --ver=v4 -o StartCalculator.js -c StartCalculator.TestClass
```