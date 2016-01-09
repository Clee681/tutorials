## Getting Started With Ruby

This is an attempt to formalize various "learning how to program" emails sent to friends.
The goals for this guide are simple:

1. Setup a proper local environment for programming
2. Highlight a few beginner friendly resources to start learning

Before we go any further, it's important to keep in mind that this is just the beginning of a journey.
There is a lot to learn regardless of how many years of experience you have.
Favor a more rigorous approach to learning.
Said differently, focus on understanding concepts rather than memorizing.
Lastly, keep in mind that most of your time spent programming will be dealing with something that is broken or not yet working.
That's the nature of building something - embrace it!

## Setting up your local environment

*This post assumes you are using Mac OS X*

1. Open the `Terminal` application
  * This is a command line interface to your computer. It's also your new home along with your text editor.

2. Install Homebrew (package manager for Mac OS X)
  * Visit `http://brew.sh/` in your favorite browser
  * Under "Install Homebrew", copy and paste the command into your terminal shell
  * The command should look something like `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

3. Check that homebrew installed successfully by running `brew --version`. You should see a version number like `0.9.5`

4. With brew successfully installed, we are going to run the following commands. `rbenv` is a tool to help us manage different ruby installations.

```bash
# Don't type the $. The $ is a common symbol to signify a shell prompt
$ brew update
$ brew install rbenv ruby-build
$ rbenv init -
```

5. Now, we're close to installing a specific version of ruby

```bash
# List all available versions:
$ rbenv install -l

# Install a Ruby version:
$ rbenv install 2.2.2
```

6. Here are some useful `rbenv` commands

```bash
# Show current ruby versions installed.
# The ruby version you are using will have an asterisk next to it
$ rbenv versions

# Switch to a specific ruby version:
$ rbenv shell 2.2.2
```

7. With the most recent version of ruby installed, we can run our first ruby program! The output of running the below command should be `Hello, world!`.

```bash
$ ruby -e "puts 'Hello, world!'"
```
