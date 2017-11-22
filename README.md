llauzau.github.io
====================

## One-Time Setup

- Run `gem install jekyll bundler`
- Run `mkdir -p ~/repos`
- Run `cd ~/repos`
- Run `git clone https://github.com/llauzau/llauzau.github.io.git`


## Local Development

- Run `cd ~/repos/llauzau.github.io`
- Run `git pull --rebase` to get the latest code from GitHub, if it fails then run `git rebase --abort` and then seek help
- Run `atom .` to open Atom or `code .` to open Visual Studio Code (if this doesn't work then just open the editor manually and then open `~/repos/llauzau.github.io` within your editor)
- Run `jekyll serve` to start your local server
- Visit [localhost.4000](http://localhost.4000) in your browser
- When making changes always refresh your browser using `[command]` + `[shift]` + `R` so the cache is cleared


## Troubleshooting

If the browser isn't reflecting your changes try restarting your local server:

- In the terminal window where you are running `jekyll serve` type `[control]` + `c` to stop your local server
- Run `jekyll serve` to start your local server again


## Publishing

- Run `cd ~/repos/llauzau.github.io`
- Run `git commit -am 'A short message describing the changes'`
- Run `git push origin master` (this will prompt you for your GitHub username and password), if this fails then you may be able to run `git pull --rebase` and then try again, if that doesn't work then type `git rebase --abort` and then seek help


## Undoing changes

Every time you run `git commit -am 'A short message describing the changes'` you create a checkpoint. If you make changes that break things you can go back to that checkpoint:

- Run `git stash -u`

If you run this command by mistake you can always undo your revert to the last checkpoint:

- Run `git stash pop`
