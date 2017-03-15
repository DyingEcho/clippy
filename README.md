# clippy: Automatically quit docs while you're working on them

Clippy is malware that, once installed and run, will occasionally quit productivity programs (such as MS Word) while you're doing work on them. This, combined with most people's tendency to only save once finished, can have huge effects on productivity - and since it adds itself to cron at first run, it is almost *impossible* to debug for anyone non-technically inclined.

Please note that this *is* active malware and so take care if testing it on your own machine. [Removal instructions] (#Removal-Instructions) are below.

## Installation instructions

1. Download the [clippy] (../../blop/clippy) executable file and save it somewhere obscure (like Application Support!)
2. Add executable permissions to it with `chmod +x ./clippy`
3. Run it (or manually add it to `crontab`. It's up to you.) You can exit with `^C` after a few seconds.
4. Enjoy.

## Removal instructions

1. Delete the script. If you don't know its location, you can check cron with `crontab -l` - it should be there somewhere.
2. Use `crontab -e` to remove the script from cron.
3. That's it. If you were looking for longer instructions, I apologise.

**Good luck. Be safe. Enjoy the rage on your friend's faces.**