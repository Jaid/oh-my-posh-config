# oh-my-posh-config

## Install

### PowerShell 7+

```bash
export reposFolder="${reposFolder:-$HOME/git}" && export ohMyPoshConfigJaidFolder="${ohMyPoshConfigJaidFolder:-$reposFolder/oh-my-posh-config}" && printf '\neval "$(~/AppData/Local/Programs/oh-my-posh/bin/oh-my-posh.exe init bash --config %s)"\n' "$(cygpath --mixed "$ohMyPoshConfigJaidFolder/src/jaid.omp.yml")" >> ~/.bashrc
```
