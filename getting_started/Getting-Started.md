**Its easy!**

---

## Installation

To download the last version of the gem:

Add ```gem 'charyf'``` to your gemfile  
or install directly using ```gem install charyf```.

Ruby version **>=2.1** is required.

### Validate the installation

Running the **charyf** command should give you similar output.

```Usage:
charyf new APP_PATH [options]


Options:
  -r, [--ruby=PATH]                          # Path to the Ruby binary of your choice
                                             # Default: /usr/bin/ruby.exe
      [--skip-gemfile], [--no-skip-gemfile]  # Don't create a Gemfile
  -G, [--skip-git], [--no-skip-git]          # Skip .gitignore file
      [--skip-keeps], [--no-skip-keeps]      # Skip source control .keep files
  -L, [--lib], [--no-lib]                    # Install Charyf as library to existing project
      [--dev], [--no-dev]                    # Setup the application with Gemfile pointing to your Charyf checkout
      [--edge], [--no-edge]                  # Setup the application with Gemfile pointing to Charyf repository
  -B, [--skip-bundle], [--no-skip-bundle]    # Don't run bundle install

Runtime options:
  -f, [--force]                    # Overwrite files that already exist
  -p, [--pretend], [--no-pretend]  # Run but do not make any changes
  -q, [--quiet], [--no-quiet]      # Suppress status output
  -s, [--skip], [--no-skip]        # Skip files that already exist

Strategies options:
  -ip, [--intent-processors=one two three]    # Set of intent intent processors to be included in installation
        Here is a list of currently available and supported intent processors,
        that can be enabled during installation
        If your processor isn't listed here, you can change it later in your project settings
        adapt
                Gem: adapt-charyf [">= 0.2"]
                Ruby wrapper around python library from mycroft [adapt]
                It uses building blocks as regexps or small expressions to define and determine intents.
                see more at: https://github.com/Charyf/charyf-adapt-processor
                                              # Default: ["adapt"]
  -sp, [--storage-provider=STORAGE_PROVIDER]  # Storage provider to be installed by default.
        Here is a list of currently available and supported storage providers,
        that can be enabled during installation
        If your provider  isn't listed here, you can change it later in your project settings
        memory
                Gem: charyf-memory-storage [">= 0.1"]
                Memory storage does not provide permanent storage as the contract may require
                but delivers enough capabilities for development and testing.
                Should not be used on production environments as it is not persisted.
                                              # Default: memory

Charyf options:
  -h, [--help], [--no-help]        # Show this help message and quit
  -v, [--version], [--no-version]  # Show Charyf version number and quit

Description:
    The 'charyf new' command creates a new Charyf application with a default
    directory structure and configuration at the path you specify.

Example
    charyf new ~/Code/Ruby/weblog

    This generates a skeletal Charyf installation in ~/Code/Ruby/weblog.
```

---
> Back: [[About]]  
> Next: [[Creating new project]]