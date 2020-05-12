# forest-linux
A linux utility that runs a command on multiple machines via ssh (with various terminal options)

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
