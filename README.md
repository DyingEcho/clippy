# clippy: Automatically quit docs while you're working on them

Clippy is malware that, once installed and run, will occasionally quit productivity programs (such as MS Word) while you're doing work on them. This, combined with most people's tendency to only save once finished, can have huge effects on productivity - and since it adds itself to cron at first run, it is almost *impossible* to debug for anyone non-technically inclined (on the other hand, if you know who Linus Torvalds is, you know how to get rid of it)

## Installation instructions

1. Download the [clippy](../../blob/master/clippy) executable file and save it somewhere obscure (like Application Support!)
2. Add executable permissions to it with `chmod +x ./clippy`
3. Run it (or manually add it to `crontab`. It's up to you.) You can exit with `^C` after a few seconds.

## Removal instructions

1. Delete the script. If you don't know its location, you can check cron with `crontab -l` - it should be there somewhere.
2. Use `crontab -e` to remove the script from cron.

**Have a lot of fun.**
