# SSH to Your EC2 Instance Instantly
SSH2 is an interactive command line tool which allows you to quickly ssh to an EC2 instance. You can select form a list of running servers under your account.

![https://raw.githubusercontent.com/soheil/ssh2/master/docs/Screen%20Shot%202015-12-06%20at%2012.47.53%20PM.png]()
![https://raw.githubusercontent.com/soheil/ssh2/master/docs/Screen%20Shot%202015-12-06%20at%2012.48.10%20PM.png]()

## Usage
`ssh2`

* Default user `ubuntu` is assumed, it can be changed at the top of this file `ssh2`

## Requirements
* [AWS CLI](https://aws.amazon.com/cli/)
* Python

## Installation
```
git clone https://github.com/soheil/ssh2.git
cd ssh2
ln -sf $(pwd)/ssh2 /usr/local/bin/
```

## Author
Soheil Yasrebi, [@soheil](https://twitter.com/soheil)
