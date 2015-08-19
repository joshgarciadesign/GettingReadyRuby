Installing Rails Environment & Useful Applications
===================

## MacOS Applications ##

1. Install Xcode
2. Install Xcode command line tools by entering the following into the Terminal.app command line:
```
xcode-select --install
```

3. Install TextMate text editor **2.0 beta**.  It is free software as of version 2.
- http://macromates.com/download

## Get TextMate.app ready for command line usage ##
1. Open TextMate.app
2. Open TextMate preferences
3. Click "Terminal" at the top of the window
4. *"Shell support not installed"* - **Click the "Install" button**
	* This will allow you to use the command "mate" from the command line in order to edit files quickly.

## Command Line Software ##
1. Install rvm ("Ruby Version Manager"):
```
$ \curl -sSL https://get.rvm.io | bash -s stable
$ $SHELL
```
2. Install ruby 2.2:
```
$ rvm autolibs read-only
$ rvm install 2.2
$ rvm use 2.2
```
3. Install Rails, haml, scss (scss is installed implicitly by installing rails):
```
$ gem install rails haml-rails
```
4. Install Sinatra.  Rails uses something called "rack" as the base of its framework.  Sinatra uses rack, as well, but with fewer components.  Installing Sinatra will provide something simple so you can play with haml and scss.
```
$ gem install sinatra sinatra-reloader
```

## HAML Test Platform ##
1. Download this git repository:
```
$ git clone https://github.com/advorak/GettingReadyRuby.git ~/Desktop/GettingReadyRuby
$ cd ~/Desktop/GettingReadyRuby
```
2. Open GettingReadyRuby in TextMate
```
$ mate ./
```
3. Back in the terminal, run the following command:
> `ruby ./sinatra.rb`
4. You can now edit the `views/index.haml` page from within textmate and see the results at http://localhost:4567/.
