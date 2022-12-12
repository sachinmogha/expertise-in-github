# get-expertise

This is a projet which contains all the folders for the technologies, which should be learned by all full stack developers

***how we setup git

created a repo in github (get-expertise)
created a new folder (get-expertise) in my machine
open command line (new terminal) in the folder(right click - new terminal at folder)

git init 

(to show hidden file run   control+shif+.)

touch .gitignore (and add node_modules/)

Now if you have not setup ssh key to the github (settings - ssh key - add a new ssh key)

https://www.youtube.com/watch?v=G14WMD8Kg3U&ab_channel=CodeWithHarry (video contains everything how to create a ssh key and add)
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/checking-for-existing-ssh-keys
https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent (this link is enough and step 2 is enough)
https://docs.github.com/en/enterprise-cloud@latest/authentication/authenticating-with-saml-single-sign-on/authorizing-an-ssh-key-for-use-with-saml-single-sign-on

to create a new ssh key (if u have already created ssh keys, no need to create again, just conpy)
$ ssh-keygen -t ed25519 -C "your_email@example.com" .  (press enter till ssh are not generate)

[below process required if your ssh config is not setup
Start the ssh agen in the background by running following command
$ eval "$(ssh-agent -s)"
> Agent pid 59566


open ~/.ssh/config

content is below of this file
Host *
  AddKeysToAgent yes
  IgnoreUnknown UseKeychain
  IdentityFile ~/.ssh/id_ed25519

if this file doesn' exist
$ touch ~/.ssh/config

Open it and paste the content as specified above
]

Now run => .pbcopy < ~/.ssh/id_ed25519.pub (copy the ssh key to clipboard)

Go to GutHub-settings-ssh key-add new shh key and add paste this key there






