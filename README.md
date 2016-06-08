# SSH to Your EC2 Instance Instantly
SSH2 is an interactive command line tool which allows you to quickly ssh to an EC2 instance. You can select from a list of running servers under your account.

![](https://raw.githubusercontent.com/soheil/ssh2/master/docs/Screen%20Shot%202015-12-06%20at%2012.47.53%20PM.png)
![](https://raw.githubusercontent.com/soheil/ssh2/master/docs/Screen%20Shot%202015-12-06%20at%2012.48.10%20PM.png)

## Usage
```
$ ssh2 1
```

```
$ ssh2 -h
Usage: ssh2 [options] [server_number]
  server_number: a numeric value corresponding to the server number
  e.g.: 'ssh2 1' will ssh into the 1st server in the list.

Options:
  -h, --help            show this help message and exit
  -x, --bust-cache      refetch servers list from AWS
  -u USER, --user=USER  provide user (default: ubuntu)
  -i IDENTITY, --identity=IDENTITY
                        provide identity file
  -p PROFILE, --profile=PROFILE
                        provide AWS profile
  --ip=IP               connect using IP instead of DNS
  -g GREP, --grep=GREP  filter the server list
```

### Filtering the list by EC2 instance name

```
$ ssh2 -g webrt

Servers list:

[1]  ec2-XX-XX-XX-XX.us-west-2.compute.amazonaws.com       webrtc-kurento

Which server would you like to connect to [1]? 

$ ssh2 -g webrt 1

Connecting to webrtc-kurento ec2-XX-XX-XX-XX.us-west-2.compute.amazonaws.com
```



## Requirements
* [AWS CLI](https://aws.amazon.com/cli/)
* Python

## Installation
```
pip install ssh2
```

or

without using Python package manager:
```
git clone https://github.com/soheil/ssh2.git
cd ssh2
ln -sf $(pwd)/ssh2 /usr/local/bin/
```

## Author
Soheil Yasrebi, [@soheil](https://twitter.com/soheil)
