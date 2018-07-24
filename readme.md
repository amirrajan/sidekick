# What is this?

It keeps an eye on files in a directory. If a file changes, this thing calls a batch file.

# How to use.

Take the files in this repo and put them in the root directory where you want file watching to occur.

Then run:

```
./sidekick.bat
```

The command above builds an exe. It's assumed that Visual Studio is installed at:

```
C:\Program Files (x86)\Microsoft Visual Studio\2017\BuildTools\MSBuild\15.0\Bin\Roslyn\csc.exe
```

Change `./sidekick.bat` if needed.

Once the app is built, it'll be started. Once started, if any file changes, `watch.bat` will be executed with the
full path of the file that was changed. From there you can delegate to whatever you'd like in a non-compiled language.
