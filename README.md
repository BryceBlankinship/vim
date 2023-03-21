# vim

Just my vim config repo

## vim-plug
Should be installed after running .vimrc, so just run :PlugInstall in .vimrc

If it isn't installed for some reason, install here:
```
curl -fLo ~/.vim/autoload/plug.vim --create-dirs \
    https://raw.githubusercontent.com/junegunn/vim-plug/master/plug.vim
```

## YCM Autocomplete

Install Homebrew:
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Install required casks/formulae:
```
brew install vim llvm cmake python go nodejs java
```

Add JDK for java support:
```
sudo ln -sfn $(brew --prefix java)/libexec/openjdk.jdk /Library/Java/JavaVirtualMachines/openjdk.jdk
```

Run the YCM setup file
```
cd ~/.vim/plugged/YouCompleteMe
python3 install.py --system-libclang --all
```




