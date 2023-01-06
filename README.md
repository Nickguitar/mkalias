# mkalias

Simple script to manage linux aliases

# Usage

Usage: `mkalias <add|ls|rm> [alias name] [alias value]`

# Examples

```
List aliases:
$ mkalias ls

Add alias:
$ mkalias ls "ls -lah"
$ mkalias copy "tee /dev/tty | xsel -ib"
$ mkalias msfconsole "sudo docker run -it --rm -p 2000:2020 metasploitframework/metasploit-framework"

Remove alias:
$ mkalias rm ls
```

# Notes

1. `mkalias ls` and `mkalias rm` will only work with aliases created via mkalias
2. If you want to make an alias containing pipes, you **must** enclose it in quotes
3. You may need to reload your shell after removing an alias