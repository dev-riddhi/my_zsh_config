# Customized zsh
Install zsh and customize it

## Install

Install zsh autosuggestions syntax-highlighting
```
sudo apt install zsh zsh-autosuggestions zsh-syntax-highlighting
```
<br>

Install starship
```
curl -sS https://starship.rs/install.sh | sh
```
<br>

Install Atuin
```
curl --proto '=https' --tlsv1.2 -LsSf https://setup.atuin.sh | sh
```

## Add autocompletion autosuggestion syntaxhighlighting

```
cd ~
```
<br>

```
mkdir .custom_git_repo
```
<br>

```
cd .custom_git_repo
```
<br>

```
git clone https://github.com/marlonrichert/zsh-autocomplete.git
```
<br>

```
nano ~/.zshrc
```
<br>

```
. "/bin"
. "/usr/bin"
. "/usr/local/bin"
eval "$(starship init zsh)"
source /usr/share/zsh-autosuggestions/zsh-autosuggestions.zsh
source /usr/share/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh
source $/.custom_git_repo/zsh-autocomplete/zsh-autocomplete.plugin.zsh
```
press ctrl+s and ctrl+x


## Vistit the url and select your prefered theme

<a href="https://starship.rs/presets/">Starship

```
starship preset catppuccin-powerline -o ~/.config/starship.toml
```

## END 
End ====================================================
