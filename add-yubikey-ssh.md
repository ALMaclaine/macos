# setup yubikey ssh

https://blog.nathanhigley.com/posts/hardwaresshkeysonmacos/
https://stackoverflow.com/questions/68573454/having-difficulty-to-get-ssh-with-a-yubikey-working-with-macos-monterey

brew install openssh 

Add to profile:
export PATH=$(brew --prefix openssh)/bin:$PATH

eval `ssh-agent`

ssh-add ~/.ssh/key
