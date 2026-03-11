# Lesson 1. Installing Crystal 

## Lesson Outcomes 
By the end of this lesson you should be able to : 
- install crystal on your operating system 
- verify the installation works 
- Run your first crystal program 

## Linux installation

### Debian based distros(ubunut/mint..etc) 
```bash
$ curl -fsSL https://crystal-lang.org/install.sh | sudo bash
# install crystal 
$ sudo apt update 
$ sudo apt install crystal
```
### Fedora 
```bash
 # Add Crystal repository
$ sudo dnf config-manager --add-repo https://dist.crystal-lang.org/rpm/
$ sudo dnf install crystal
```
### Arch Linux
```bash
$ sudo pacman -S crystal
```
### Other Linux distros
 **visit** [crystal](crystal-lang.org/install)
## MacOs 
### Using Homebrew(recommended)
```bash
# Install homebrew if you don't have
$  /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# Install Crystaltl
$ brew install crystal
```
### Using Macport
```bash 
$ sudo port install crystall
```
## Windows 
 support for windows is still in **preview** 
download the .exe file [install.exe](https://crystal-lang.org/install/on_windows/) 

# Verifying Installation 
 After your installation must have been successful open a terminal/shell
then run 
```bash
$ crystal --version
```
you should see similar output to this: 
```bash
Crystal 1.16.0 (2025-05-06)

LLVM: 15.0.7
Default target: x86_64-pc-linux-gnu
```
## Your first crystal project 
- create a file named hello.cr
  ```bash
  $ touch hello.cr
  ```
  - in your code editor open the hello.cr or using nano
    ```bash
    $ nano hello.cr
    ```
  ```crystal
  # hello.cr
  puts "Hello world!"
  ```
  - Run it
  ```bash
  $ crystal hello.cr
  ```
  expected output
  ```bash
  Hello world!
  ```
## Compiling to binary 
crystal can also compile your code to standalone executables(binary)
```bash
$ crystal build hello.cr -O hello
# then run the hello file
$ ./hello
```

## Troubleshooting 
command not found after installation 
- Restart your terminal
- make sure that installation path is in your PATH
### Permissions Issue
if you get permission errors 
```bash
# not recommended to use sudo with crystall command
# check file permission
$ chmod +x hello.cr
```
## Knowledge Check
- what command checks your crystall version?
- how do you run a **crystal** file without compiling?

## Additional Resources 
- [official crystal installation guide](https://crystal-lang.org/install/)

  


  















