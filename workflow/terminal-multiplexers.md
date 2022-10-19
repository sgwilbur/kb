# Terminal Multiplexers

Help with organizing and persisting terminal sessions for one or more systems.

# What I use

I was super sold on using [`screen`](../../tools/screen.md) only and it totally slaps on it's own.

My challenge was trying to use `screen` both locally and remotely. So when that need arose I was stuck, yes you can use screen in screen if you need to.

My preference is to add `Tmux` to the mix, I found an idea for how to use them both together from another ask out in the world. I actually found that I liked Tmux more as my primary interface then I use screen within.

 They have non-conflicting control modifier keys, so no double/triple tap non-sense, but I have a double set of commands that are similar but not the same.

# Scenarios

1. Running a long job via the cli that will terminate if the current session is broken. (backups, scans, viewing logs)

*Using a multiplexer allows for terminal processes to be tied to a long running processess, allowing for terminals to remain open if when you disconnect as their process does not terminate when a connection ends. The service remains running on the system and will be ready to resume an active session when the connection is restored.

1. Having multiple sessions open to the same machine.

*While troubleshooting on a headless/gui-less machine to do something like `tail` multiple logs concurrently for multiple services.*

1. Pair programming/troubleshooting/experimenting

* Having a multiplexer in the middle of standard session, allows for more than one parcipant to ser
*


# Example tools

 * [Screen](../tools/screen.md)
 * [TMux](../tools/tmux.md)

