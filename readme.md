# oh-my-posh-config

## Installation

### Bash (from Git for Windows)

```bash
export reposFolder="${reposFolder:-$HOME/git}" && export ohMyPoshConfigJaidFolder="${ohMyPoshConfigJaidFolder:-$reposFolder/oh-my-posh-config}" && printf '\neval "$(%s init bash --config %s)"\n' "$(cygpath --mixed "$(which oh-my-posh)")" "$(cygpath --mixed "$ohMyPoshConfigJaidFolder/src/jaid.omp.yml")" >> ~/.bashrc
```

### zsh (from Git for Windows)

```bash
export reposFolder="${reposFolder:-$HOME/git}" && export ohMyPoshConfigJaidFolder="${ohMyPoshConfigJaidFolder:-$reposFolder/oh-my-posh-config}" && printf '\neval "$(%s init zsh --config %s)"\n' "$(cygpath --mixed "$(which oh-my-posh)")" "$(cygpath --mixed "$ohMyPoshConfigJaidFolder/src/jaid.omp.yml")" >> ~/.zshrc
```

### PowerShell 7

```bash
export reposFolder="${reposFolder:-$HOME/git}" && export ohMyPoshConfigJaidFolder="${ohMyPoshConfigJaidFolder:-$reposFolder/oh-my-posh-config}" && export powershellProfileFolder="${powershellProfileFolder:-$HOME/Documents/PowerShell}" && mkdir --parents "$powershellProfileFolder" && printf '\nInvoke-Expression (%s init pwsh --config "%s")\n' "$(cygpath --mixed "$(which oh-my-posh)")" "$(cygpath --mixed "$ohMyPoshConfigJaidFolder/src/jaid.omp.yml")" >> "$powershellProfileFolder/profile.ps1"
```
