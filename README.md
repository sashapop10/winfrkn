# Just my GoodbyDPI setup for Windows machines

## Installation

> [!CAUTION] 
> 
> Remind to run all `*.cmd` files as admin, this will be security issue but who cares for windows systems, right?

1. Download repository from [here](https://github.com/sashapop10/winfrkn/archive/refs/heads/main.zip) and unpack it to the Desktop
2. Run `update.cmd` script
3. Run `test.cmd`, dont close yet - test how it works with youtube in incognito mode.
    1. If it works out of the box - you are happy one, skip to chapter **4**  
    2. If you unlucky one, you need to open same file at your favorite editor, like windows notepad 
    3. You need to find `start "" goodbyedpi.exe` code fragment
    4. Try to replace flag `-9` with other possible options: 
        - `-6 -e1` 
        - `-5 -e1`
        - `-9 -e1 -f1` 
        - `-9` 
    5. If blind configuration doesn't work, try to look at the [source of truth](https://github.com/ValdikSS/GoodbyeDPI/issues/378https://github.com/ValdikSS/GoodbyeDPI/issues/378);

4. (optional) If you want to run this at startup:
    1. Close current script if such is running 
    2. Open `setup.cmd` with your facvorite text editor
    3. You need to find `sc create "GoodbyeDPI" binPath=` code fragment
    4. Do same thing as you already did at `step 3`
    5. Run `setup.cmd`

## FAQ

- ### Have a problem ? Try the source of truth:
    #### [Repository origin](https://github.com/ValdikSS/GoodbyeDPI) | [Topic for RU](https://github.com/ValdikSS/GoodbyeDPI/issues/378https://github.com/ValdikSS/GoodbyeDPI/issues/378)
