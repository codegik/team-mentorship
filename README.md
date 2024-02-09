# Team mentorship

This is a tool belt to help me in daily bases work as a software engineer mentor.

## Requirements
- Git client

## Setup
Just need to create a list of repositories you want to watch in this config file `~/.config/team/repos`.

```bash
mkdir -p ~/.config/team
echo "https://github.com/codegik/pocs.git" >> ~/.config/team/repos
```

## team-commits

This tool shows the last commit from yesterday for each engineer.

Ihe status `NOT-OK` means nothing was commited yesterday.

The status `OK` means something was commited yesterday, and also print the last commit url.


Example:
```bash
./team-commits
Downloading codegik/pocs ...
Downloading engineer123/pocs ...

User repo          Status  Commit url
codegik/pocs       NOT-OK  https://github.com/codegik/pocs/commit/
engineer123/pocs   OK      https://github.com/engineer123/pocs/commit/12345678909058ae72b4c0c284110e5539b7f69a

```


