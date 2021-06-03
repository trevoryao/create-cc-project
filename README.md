# create-cc-project
This is a handy script I created for creating new C++ projects compiled using a Makefile,
which I made accessible for beginners. It behaves similar to `npm-create-react` tool for
react projects.

This will create a C++ Project template in the given directory with root 'project-name',
with a Makefile & .gitignore, and the binary and source files as given in the arguments.
It will also initialise git repo if git is installed

## Installation
You can install the tool using `curl`.
```
curl https://raw.githubusercontent.com/trevoryao/create-cc-project/master/create-cc-project -o $HOME/bin
```
`wget` can also be used. If installing on a virtual machine or container, the `-k` flag 
may have to be used.

## Usage
```
create-cc-project [options] <project-name>

options:
  -h | --help				Help Screen
  -d | --directory			Directory to create project root in (defaults to current dir)
  -c | --compiler <arg>		C++ Compiler [g++, clang++, etc...]
  -s | --std <arg>			C++ std (defaults to C++14)
  -e | --ext <arg>			C++ file extension (defaults to .cc)
  -b | --bin <arg>			name of file to store binary files in (defaults to bin)
  -s | --src <arg>			name of file to store source files in (defaults to src)
  -u | --remote-url <arg>	git remote url (optional, will initialise empty repo)
```
