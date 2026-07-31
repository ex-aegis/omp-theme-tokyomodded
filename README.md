# A simple custom modification I've made of the Tokyo theme from the oh-my-posh project by _JanDeDobbeleer_.

## **How to use the theme:**

### Powershell

Inside your notepad Profile:
```
notepad $PROFILE
```
Then put this:
```
if (Test-Path alias:\r) { Remove-Item alias:\r }
oh-my-posh init pwsh --config ~/tokyomodded.omp.json | Invoke-Expression
```
### Bash

In your ~/.bashrc file:
```
[[ $(alias r 2>/dev/null) ]] && unalias r
eval "$(oh-my-posh init bash --config ~/tokyomodded.omp.json)"
```

### More

https://ohmyposh.dev/docs/installation/customize
