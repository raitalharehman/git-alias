# git-alias

### For Windows
>copy these lines below and paste in .gitconfig file on `C:\Users\{user}`.

### For MacOs
>copy these lines below and past in .gitconfig file on `~`.


```
[alias]
	hide = update-index --assume-unchanged
	unhide = update-index --no-assume-unchanged
	co = commit
	st = status
	ch = checkout
	di = diff --color-words
	br = branch
    	ph = push
	pl = pull
	cob = checkout -b
	cm = !git add -A && git commit -m
	fc = !git fetch && git checkout
	save = !git add -A && git commit -m 'SAVEPOINT'
	wip = commit -am "WIP"
	fire = !git save && git ph 
	lg1 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%s%C(reset) %C(dim white)- %an%C(reset)%C(bold yellow)%d%C(reset)' --all
	lg2 = log --graph --abbrev-commit --decorate --format=format:'%C(bold blue)%h%C(reset) - %C(bold cyan)%aD%C(reset) %C(bold green)(%ar)%C(reset)%C(bold yellow)%d%C(reset)%n''          %C(white)%s%C(reset) %C(dim white)- %an%C(reset)' --all
	lg = !"git lg1"
  ```
