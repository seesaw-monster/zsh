# Zsh Settings
## File directory
```
cd $HOME/.config
git clone git@github.com:seesaw-monster/zsh.git
```
## Setting Activation
```bash
echo 'source $HOME/.config/zsh/myzshrc' >> ~/.zshrc
source ~/.zshrc
```

## Plugin manager
install
```bash
brew install zplug
```
インストール後次のコマンドをhomebrewに言われるがまま~/.zshrcに追記
~/.zshrc
```bash
export ZPLUG_HOME=$(brew --prefix)/opt/zplug
source $ZPLUG_HOME/init.zsh
```
次のコードも追記しないとコマンドが認識されなかった
```bash
if [ -f $ZPLUG_HOME/init.zsh ]; then
    source $ZPLUG_HOME/init.zsh
fi
```
