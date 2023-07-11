# mac-react-native-setup
Real setup from scratch

1) Install Brew follow the: https://brew.sh/ <br>
   just run: $ /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
2) Meanwhile you can start the download of xcode: https://xcodereleases.com/
3) Install rben using brew: $ brew install rbenv
4) After the installation completes, you need to initialize rbenv by adding the following command to your shell profile file (e.g., ~/.bash_profile, ~/.zshrc, or ~/.bashrc):<br>
   $ if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi<br>
   or just run: $ echo 'if which rbenv > /dev/null; then eval "$(rbenv init -)"; fi' >> ~/.bash_profile<br>
   $ source ~/.bash_profile<br>
   Maybe also it's necessary to add these lines:<br>
     export PATH="$HOME/.rbenv/bin:$PATH"<br>
     eval "$(rbenv init -)"<br>
   and run again: $ source ~/.bash_profile
5) Before install/upgrade  ruby runs: $ brew update && brew upgrade ruby-build
6) Se the available versions of ruby: $ rbenv install --list
7) Install ruby through rbenv: $ rbenv install <version>
8) Set the version as local or global: $ rbenv global <version> or $ rbenv local <version>
9) Install gem, I usually use sudo: $ sudo gem install cocoapods<br>
   Sometimes it's necessary to add a activesupported version<br>
   $ sudo gem install activesupport -v <version> e.g. $ sudo gem install activesupport -v 6.1.7.4<br>
   $ sudo gem install cocoapods
11) Set the Xcode version: $ sudo xcode-select -s <path to your xcode> e.g. (sudo xcode-select -s /Applications/Xcode_14.app)<br>
    To verify your xcode version: $ xcodebuild -version
12) Install React-native CLI https://reactnative.dev/docs/environment-setup?guide=native&os=macos&platform=ios
13) $ brew install node
14) $ brew install watchman
15) Remove previous installation: $ npm uninstall -g react-native-cli @react-native-community/cli
16) New project: $ npx react-native@latest init AwesomeProject
17) CD AwesomeProject and: $ npm start
