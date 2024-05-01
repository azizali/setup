# Setup Preferences for my mac

### Show hidden files
Run these two commands:
1. `defaults write com.apple.Finder AppleShowAllFiles true`
1. `killall Finder`

### Install Apps
#### General
- https://brew.sh/
- https://brave.com/download/
    sync bookmarks
- `brew install spectacle workflowy iterm2 sourcetree postman git nvm`
	- https://www.spectacleapp.com/ (brew)
	- https://workflowy.com/downloads/windows/ (brew)
 	- https://iterm2.com/ (brew)
	- https://www.sourcetreeapp.com/ (brew)
	- https://www.postman.com/ (brew)
 	- Node version manager
  	- git  
- https://apps.apple.com/us/app/slack-for-desktop/id803453959?mt=12
- https://www.google.com/drive/download/ 

#### Developer
- https://code.visualstudio.com/
- https://www.docker.com/products/docker-desktop
- https://nosqlbooster.com/downloads

#### Brew install
-  `brew install git`
-  

## Terminal
### iterm2 natural escaping option + arrow
https://apple.stackexchange.com/questions/154292/iterm-going-one-word-backwards-and-forwards
1. Go to Preferences... > Profiles > Keys (not Preferences... > Keys)
2. Make a new profile and set it to default
3. Key mapping
4. Press Presets...
5. Select Natural Text Editing
6. Remove

### ZSH setup
https://ohmyz.sh/#install

### Git setup
SSH keys
git config
`code ~/.gitconfig`
contents of `.gitconfig`
```
[user]
	email = aziz@.org
	name = Aziz Ali
[core]
	excludesfile = /Users/azizali/.gitignore_global
[difftool "sourcetree"]
	cmd = opendiff \"$LOCAL\" \"$REMOTE\"
	path = 
[mergetool "sourcetree"]
	cmd = /Applications/Sourcetree.app/Contents/Resources/opendiff-w.sh \"$LOCAL\" \"$REMOTE\" -ancestor \"$BASE\" -merge \"$MERGED\"
	trustExitCode = true
[alias]
	b = branch
	
	co = checkout
	cob = checkout -b
	
	com = commit -m
	
	pl = pull
	plo = pull origin
	plom = pull origin main
	
	ps = push
	pso = push origin
	psom = push origin main

	r = rebase
	ri = rebase -i
	riom = rebase -i origin/main

	rsh = reset --hard
	rss = reset --soft
```


## VS CODE SYNC settings

## Development
### Node & family
**nvm** https://github.com/nvm-sh/nvm#installing-and-updating
**node** `nvm install node`
**yarn** `npm install -g yarn`
