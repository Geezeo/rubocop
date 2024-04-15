# RuboCop Configuration Repository
## Overview
This repository contains the shared RuboCop configurations used across all our Ruby projects. RuboCop is a Ruby static code analyzer (linter) and formatter that enforces many of the guidelines outlined in the community Ruby Style Guide.

The purpose of this repository is to maintain a consistent coding style and improve the quality of code across all our projects. It includes a base configuration file that applies universally to all projects, with the ability to extend or override these settings for specific projects.

## Getting Started
### Prerequisites
* Ruby (version specified by .ruby-version)
* RuboCop gem installed in your projects

### Using the Configurations
To use these configurations in your project, add this line to your project's Gemfile:

```ruby
gem 'rubocop', require: false

```

Then, add a .rubocop.yml file to your project's root directory with the following line to inherit from the shared configuration:

```
inherit_from:
  - https://raw.githubusercontent.com/Geezeo/rubocop/develop/.rubocop.yml
```

### Updating Configurations
To update the RuboCop configuration in this repository create a new branch, make changes, and push them for review. Please unsure the entire team is in agreement to the changes as this affects how we all code.