# sn
Simple Notes using fzf



Simple Note Taking inside the Terminal

Dependence fzf

Use your own text editor; sn.sh script is using micro as it's text editor. You can edit that part to use vim or emacs.

You can use any text editor that you like. I'm using micro. Just use this script and edit "$Editor" to "micro" or any other editor you prefer. I name my sn.sh sn for simple note. I put this script in a directory name .notes. I also created a .md file call sn.md and just added MY Notes in the file. This is where I'm going to add my notes. I even can created other files name them by dates, events, or anything else and search in each one very easy. Now in the script I'm using a application call fzf. To install just do this

git clone --depth 1 https://github.com/junegunn/fzf.git ~/.fzf

Enter and Enter on the next prompt to install. Then I just answer y(yes) on all three questions. Now one more step an alias in bash. My .bash_aliases file I added this.

alias sn="cd ~/.notes && ./sn.sh"

So when I type out sn in my terminal. fzf is running inside the .notes directory. Just type out sn.md **{TAB} To get the auto completion set. Next time you run sn. sn.md is highlighted. And when you press Enter your in your text editor. Now add your notes and save. Esc to exit fzf. And I'm back where I left off inside the terminal.
