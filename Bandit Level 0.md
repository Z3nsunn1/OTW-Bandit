
## Level Goal

The goal of this level is for you to log into the game using SSH. The host to which you need to connect is **bandit.labs.overthewire.org**, on port 2220. The username is **bandit0** and the password is **bandit0**. Once logged in, go to the [Level 1](https://overthewire.org/wargames/bandit/bandit1.html) page to find out how to beat Level 1.

## Commands you may need to solve this level

[ssh](https://man7.org/linux/man-pages/man1/ssh.1.html)

## Helpful Reading Material

- [Secure Shell (SSH) on Wikipedia](https://en.wikipedia.org/wiki/Secure_Shell)
- [How to use SSH on wikiHow](https://www.wikihow.com/Use-SSH)
---
### Helpful Links
[Explain Shell](https://explainshell.com/) - Get detailed explanation on linux commands.

### Explanation
We need to log in using SSH so let's take a look at this command, either via explainshell by typing SSH or using the command below in your Linux terminal:

```bash
man ssh
```

Here we can see a brief description for the command:

![[Pasted image 20230917122442.png]]

![[Pasted image 20230917122611.png]]

So, from reading the description we can derive that the syntax to use ssh would be:

```bash
ssh <options><hostname> #where options can be anything or nothing, and hostname is the name or IP where you would want to connect.
```

If you would like to connect to a specific user you can run the syntax as follows, once you connect ssh will prompt you for that users password:

```bash
ssh <options> <username>@<hostname>
```

### Solution

So we need to connect to a specific user in a specific port, let's run the command:

```bash
ssh -p 2220 bandit0@bandit.labs.overthewire.org 
```

You can type yes to continue establishing the connection

![[Pasted image 20230917123644.png]]

There you go you are in, just type the password given which is bandit0!

![[Pasted image 20230917123747.png]]