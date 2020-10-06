# pwdgen

Password generator for the command line, written in python

## What does it do?

Well... it generates passwords. There are currently 4 types: pin, password, crypt and aaa

### pin

Generates a pin with digits between 0 and 9 (0 1 2 3 4 5 6 7 8 9)

### password

Generates a password. It doesn't include all special characters, only "!@#\$%&\*()\_-+={[]}|:;<,>.?/"

### crypt

contains numbers, ascii letters and punctuation

### aaa

ÀâÃÀÅAÃÁÃAÆÀÅÃÀãāāÁâäáÀåäaÁÃāäÆÂaÅâååàåáåâāÀAàâÁÃà

## Installation

You need:

- python 3
- pip3
- 1 minute

You could just leave the file here, navigate to this directory and run `python3 pwdgen.py`, but that's inconvenient.
I copied the file to `/usr/local/bin` and removed the `.py` file extension so i can run `pwdgen` from everywhere. Might require a terminal relaunch, idk

To copy the file to `/usr/local/bin`, run `sudo cp ./pwdgen.py /usr/local/bin/pwdgen`
DISCLAIMER: I tested this on my machine, running macOS. idk if this is gonna work on other systems. it shouldn't break anything, but don't blame me if it does :)

And yeah, you need the dependencies. Run `pip3 install -r requirements.txt` from this directory and it should automagically install all dependencies.

## Usage

`pwdgen -pwd|-pin|-crypt|-aaa [-cp] -l L`

Everything in [] is optional
When there's a horizontal line (|), you can choose

- `-pwd`

  - generates a password

- `-pin`

  - generates a pin

- `-crypt`

  - generates a random string

- `-aaa`

  - ÅÁäãæäaàåaÃAÄáÂæaĀÂàäÃååáÀĀĀÄÅàaÆAAÄâaaâåäàAæÃÁāÄĀ

- `-cp`

  - copies the result

- `-l L`
  - length of the string (L = integer)
  
# Contribute

If you can improve pwdgen (or fix the shitty code I wrote), feel free to create a PR!<br/>
I don't think i need a code of conduct or contributing file (even though github wants me to create one), just don't insult anyone and be nice!

# License

This project is licensed under the MIT License. Read [LICENSE](LICENSE) for more information
