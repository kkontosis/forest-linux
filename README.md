# forest-linux
A linux utility that runs a command on multiple machines via ssh (with various terminal redirection capabilities).
- Option to run interactive commands with/without hidden input, e.g. change a password for a user across many nodes.
- Includes a customizeable set of scripts that run a series of interactive operations on the host machines automatically, e.g. user creation.
- Experimental ability to run a command asynchronously, at first boot, if one or more machines are down or fail to execute the given command.


## Example

/etc/forest/node:
```bash
node01
node02
node03
```

Run the command:
```
forest sudo apt-get install vim
```

Then press `'y' <enter>` once, and the keystroke will be forwarded to all the nodes.

Congratulations, you just installed `vim` to 3 nodes at once!

## Usage

The help is embedded in the utility with `forest --help`.
