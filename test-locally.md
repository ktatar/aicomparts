To test your al-folio personal website locally on macOS, you'll need to set up your environment for Jekyll, the static site generator that al-folio uses. Here’s a step-by-step guide to help you run your website locally:

# Step 1: Install Homebrew
First, you'll need Homebrew, which is a package manager for macOS. It will help you install Ruby and Jekyll easily. Open the Terminal app and run:

bash
Copy code
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"


# Step 2: Install Ruby
al-folio runs on Ruby, so you'll need to install a version of Ruby via Homebrew (macOS comes with Ruby, but it’s a good practice to use a version manager like rbenv to avoid permissions issues):

bash
Copy code
brew install rbenv
rbenv init
Follow the instructions on the terminal to set up rbenv. You'll likely need to add eval "$(rbenv init -)" to your shell configuration file (.bash_profile, .zshrc, etc.).

Then, install Ruby with rbenv:

bash
Copy code
rbenv install 3.1.2  # Check for the latest version that's compatible with Jekyll
rbenv global 3.1.2
ruby -v  # Check Ruby version

# Step 3: Install Bundler and Jekyll
Now that Ruby is installed, you can install Bundler and Jekyll:

bash
Copy code
gem install bundler jekyll

# Step 4: Clone Your al-folio Repository
If you haven’t already, clone your al-folio repository from GitHub to your local machine:

bash
Copy code
git clone https://github.com/username/al-folio.git
cd al-folio
Replace https://github.com/username/al-folio.git with the actual URL of your repository.


# Step 5: Install Dependencies
Inside your project directory, install the Ruby gems specified in your Gemfile:

bash
Copy code
bundle install


# Step 6: Run Jekyll Locally
Start the Jekyll server:

bash
Copy code
bundle exec jekyll serve

# Step 7: View Your Site
Open a web browser and go to http://localhost:4000 to see your site in action.

Troubleshooting Common Issues
Dependency Problems: If bundle install fails, check the error message to see which gem is causing the issue. Sometimes you may need to install additional libraries on your system.
Port Already in Use: If you get an error that the port is already in use, you can change the port by running bundle exec jekyll serve --port 5000.
By following these steps, you should be able to test and develop your al-folio personal website locally on your macOS system.