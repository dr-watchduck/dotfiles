### ref github
https://github.com/craftzdog/dotfiles-public


### 다음 순서로 실행. 복붙 ㄴㄴㄴㄴㄴㄴ
```sh
git clone https://github.com/craftzdog/dotfiles-public.git ~/.dotfiles
brew install tmux neovim
brew install iterm2 --cask
brew tap homebrew/cask-fonts
brew install --cask font-hack-nerd-font 
brew install exa
brew install peco
brew install ghq
sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"

https://github.com/naver/d2codingfont/releases/tag/VER1.3.2 << zip 파일 다운로드 후. All 폴더에 들어가. 서체 설치 하기.

ln -s ~/.dotfiles/.tmux.conf ~/.tmux.conf
ln -s ~/.dotfiles/.tmux.conf.osx ~/.tmux.conf.osx
ln -s ~/.dotfiles/.tmux.powerline.conf ~/.tmux.powerline.conf

tmux source-file ~/.tmux.conf
tmux source-file ~/.tmux.conf.osx
tmux source-file ~/.tmux.powerline.conf

ln -s ~/.dotfiles/.zshrc ~/.zshrc
ln -s ~/.dotfiles/agnoster.zsh-theme ~/.oh-my-zsh/themes/agnoster.zsh-theme

source ~/.zshrc
```

### 세션 생성
```sh
tmux
tmux new
```

### 세션 목록
```sh
tmux ls
```

### 세션 종료
```sh
tmux kill-session -t [index]
```

### 세션 재접속
```sh
tmux attach -t 0 [index]
```

### 세션 나가기
```sh
ctrl + p, d
```

### window 생성
```sh
ctrl + p, c
```

### window 종료
```sh
ctrl + d
```

### window 전환
```sh
ctrl + p, [0~9]
ctrl + p, p
```

### window 변경
```sh
ctrl + p, h or j or k or l
```