python_de4py

this project has been officially archived. It has been a rewarding experience to develop and share this project with the community. However, I’ve noticed that many users lack the necessary coding or reverse engineering experience to fully benefit from the project. This has led to an increase in basic questions and issues that detract from the project's original intent.

# de4py



**important note: IF YOU ARE A SKID AND DON'T KNOW HOW TO CODE OR USE AI TO CODE AND HAVE NO EXPERIENCE AT ALL THEN THIS TOOL IS NOT FOR YOU !!!**

**what is de4py?**

De4py are an Advanced python deobfuscator with a beautiful UI and a set of Advanced features that enables malware analysts and reverse engineers to deobfuscate python files and more. this project is maintained by me ([Fadi002](https://github.com/Fadi002)) and my friend [AdvDebug](https://github.com/AdvDebug)。

## Features



| Feature                 | Function                                                     |
| ----------------------- | ------------------------------------------------------------ |
| Deobfuscation           | De4py support some popular obfuscators, like: Jawbreaker, BlankOBF, PlusOBF, Wodx, Hyperion, [pyobfuscate.com](https://pyobfuscate.com/) obfuscator |
| Pycode Execution        | Executing your python code inside the process which can be useful in many cases to make the program do something you want to make it do, for example if the program have licensing and it calls the real "main" only if you bought the program you can call it directly. |
| Strings Dump            | Dumping Strings in the python process and saving it as a file which can be pretty useful to extract data from memory such as webhooks. |
| Removing Exit Function  | Removing the exit function which can be extremely useful if the python program tried to exit itself if it found a debugger or a VM |
| Getting All Functions   | Getting all functions inside the python process which can be really useful when trying to modify a python function in memory |
| Pyshell GUI             | Custom GUI to make it easy to execute python code inside the desired process. |
| GUI and Console Support | De4py supports both console and GUI, but why use console when you can have a nice-on-the-eyes GUI, am i right? ;) |
| File Analyzer           | an analyzer that have many features like detecting if the python program is packed and tries to unpack it if it was using pyinstaller for example, it also got a feature that shows either all strings or suspicious strings (suspicious strings like: IPs, websites, and "token" "discord" "leveldb" strings and other suspicious strings in the file) and shows them in a nice output window. |
| Behavior Monitoring     | De4py can monitor python processes and see if they opened any files handles, opened a process, wrote/readed the memory of other processes and also monitoring if the process terminated other processes, in addition to sockets monitoring (including the size of data that is being sent and the ip that is being sent/recieved from) along with dumping socket content to a file and dumping OpenSSL encrypted content decrypted into a file, and PYC dumping. |
| Plugins system          | You can add plugins to de4py to customize the theme or add custom deobfuscators [plugins repo and docs here](https://github.com/Fadi002/de4py-plugins-repo) |
| API system              | You can use de4py features such as deobfusctor engine and pyshell in your own tools [API docs here](https://github.com/Fadi002/de4py/tree/main/api) |