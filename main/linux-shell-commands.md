# Linux Commands

## General Commands

- `sudo chown -R <user> <dir>`

## Shell Tricks

- `$(*)` where * is a command, will spawn a sub-process to free up the main bash process

## pushd and popd

- `pushd <options> <dir>` adds the current dir to the `dirs` stack then navigates to the passed dir
- `popd <options>` removes the most recenet dir for the dir stack and navigates to it
  - `-3 +5` as an option to `popd` removes the nth item from the stack from the bottom (-3) or top (+5)
- `dirs` outputs all directories on the stack. Usefult for piping to stdin in other commands

## Check For Process Before Executing Process in Bash

```bash
if [[ $(ps -a | grep anydesk) ]]; then
  echo "Anydesk instance found";
else
  echo "No Anydesk Instance found";
  anydesk;
fi
```
