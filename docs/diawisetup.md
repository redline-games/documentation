# Diawi Setup

---

Diawi is a platform that allows us to easily share builds for testing.

This document provides a brief setup guide to get started.

---

### Install homebrew

-- *Skip this step if homebrew is already installed* --
<br>

Homebrew is a package management software that will easily let you install softwares on your mac.

To install homebrew, open Terminal and run the following command
```text
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

Next, run the following commands one by one to add the path for homebrew
```text
(echo; echo 'eval "$(/opt/homebrew/bin/brew shellenv)"') >> /Users/[YOUR_USER]/.zprofile
```

```text
eval "$(/opt/homebrew/bin/brew shellenv)"
```

---


### Install python3

You can check if you already have python3 installed using the following command
```text
python3 --version
```

If python3 is not installed, you can install it using homebrew
```text
brew install python
```

Once installation is complete you can verify it again using
```text
python3 --version
```

---

### Edit Path for zsh

In your Finder window, navigate to
```text
Users/[YOUR_USER]
```

Enable hidden files using the keys
```text
cmd + shift + .
```

Once hidden files are visible, look for a file by the name ".zshrc"

If such a file does not exist, you can download one from here and paste it in the folder

If the file exists, open it in TextEdit and add the following lines to set PATH for python3 and also set aliases for python and pip
```text
export PATH="/opt/homebrew/bin:$PATH"
alias python="python3"
alias pip="pip3"
```

Finally to update and save the .zshrc file, run
```text
source ~/.zshrc
```

Now you can run these commands one by one
```text 
python —-version
```
```text 
pip —-version
```
They should return python3 and pip3 versions respectively as we have added aliases for them

---

### Install pip

-- *Skip this step if pip is already installed* --
<br>

Get the latest python3 installation package from [here](https://www.python.org/downloads/macos/ "pip")
