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
  * This is a command line interface to your computer. You'll be spending a lot of time here.

2. Install Homebrew (package manager for Mac OS X)
  * Visit `http://brew.sh/` in your favorite browser
  * Under "Install Homebrew", copy and paste the command into your terminal shell
  * The command should look something like `ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"`

3. Check that homebrew installed successfully by running `brew --version`. You should see a version number like `0.9.5`

4. With brew successfully installed, we are going to run the following commands.

  ```bash
  # Don't type the $. The $ is a common symbol to signify a shell prompt
  $ brew update
  $ brew install rbenv ruby-build
  $ rbenv init -
  ```

  *Note: `rbenv` is a tool to help us manage different ruby installations.*

5. Now, we're close to installing a specific version of ruby

  ```bash
  # List all available versions:
  $ rbenv install -l

  # Install a Ruby version:
  $ rbenv install 2.2.2
  ```

6. Here are some useful `rbenv` commands

  ```bash
  # Show current ruby versions installed
  # The ruby version you are using will have an asterisk next to it
  # Notice that there is a system ruby! Macs come with a ruby version pre-installed
  # We actually used the system ruby to install homebrew earlier
  $ rbenv versions

  # Switch to a specific ruby version:
  $ rbenv shell 2.2.2
  ```

7. With the most recent version of ruby installed, we can run our first ruby program! The output of running the below command should be `Hello, world!`.

  ```bash
  $ ruby -e "puts 'Hello, world!'"
  ```

8. Very soon, you'll be writing much larger programs. Consequently, executing ruby code as a string argument to the ruby interpreter will become impractical. Instead, we'll write code in a separate text file, and pass the file to the ruby interpreter. A text editor will allow us to edit plain text. Two popular text editors today are listed below. Choose whichever one you like.

  * [Sublime Text 3](http://www.sublimetext.com/)
  * [Atom](https://atom.io/)

9. You'll also need a Github account. Sign up for a free account [here](https://github.com/). Github is a popular site for sharing and collaborating on projects. This tutorial is actually hosted by github. If you see an error in this guide or have something you'd like to add, just file a new issue under the project, and I'll be notified. We can then work together to make this guide better.

## Learning Resources

After setting up your local environment, I recommend reading through Zed Shaw's [Learn Ruby the Hard Way](http://learnrubythehardway.org/book/). It's free, and will have you writing a lot of small programs. Don't skip the exercises, and don't copy and paste!
