# S-PHP :- Shell script to switch php versions on linux.

Using **a Linux** system with multiple **PHP** versions installed by apt? Now you may look for an easy way to switch between multiple PHP versions without executing multiple commands manually, Well we can use [S-PHP](https://vinugawade.github.io/s-php) for that.

### How to install on Linux:-

Clone the [S-PHP](https://github.com/vinugawade/s-php) repository to your local machine using the command.

```bash
git clone https://github.com/vinugawade/s-php.git
```

Move the shell script file to `/usr/local/bin` location or use the command.

```bash
sudo mv `/location/of/file` /usr/local/bin
```

Allow everyone to execute the script using the command.

```bash
sudo chmod +x `/location/of/file`
```

OR

```bash
sudo chmod 0755 `/location/of/file`
```

Add `usr/local/bin` to your `$PATH`. if you use the `Bash` shell, Then you can do this by using the command.

```bash
export PATH=$PATH:/usr/local/bin
```

OR

```bash
export PATH=$PATH:`/location/of/file`
```

This will set the variable name:- potentially in a file called `~/.bash_profile`**,** `~/.bashrc` and `~/.profile`**.** The difference between these files is (primarily) when they get read by the shell. If you're not sure where to put it, Then `~/.bashrc` is a good choice.

**Note:- You may need to restart your shell for this to take effect.** 

### How to use the script:-

```bash
s-php 7.4
```

OR

```bash
s-php 8.0
```

This will change your PHP execution file of the system as well as the apache server's PHP config to use a different version.

### Mac User?

You can check this [sphp](https://github.com/jschaedl/sphp-osx) repository as an alternative script for Mac OS.​