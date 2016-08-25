# Generate modules classpath

This script adds to liferay eclipse project all `src` directories from osgi modules 

## Installation
Just copy the sh files to your system

For windows users: you can launch the script from cygwin

## Usage
1. Important: Before using the script, execute `ant all` in order to download all `jar` dependencies
2. Execute `/path/generate_modules_classpath.sh [project-directory]`
   * project-directory: directory where eclipse project is located. (optional parameter, the current directory by default)
3. The script will make a backup of original eclipse `.classpath` in `.classpath_backup` and `.classpath` will be populated with all src and jar files from osgi modules

In case you also want to add tests classes to classpath, use `generate_modules_classpath_with_tests.sh`
 