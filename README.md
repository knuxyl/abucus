# abucus
Shell script for managing, building, and running git projects

Should be compatible with dash, bash, ash, and I believe anything that supports the original shell scripting language.

Can use a .conf file (optional) in the same directory as abucus named abucus.conf. Can change in script.

Very simple shell script, no complicated mess. Basic grep and sed commands.

Abucus creates scripts for each project cloned that is independent or can be ran from the main abucus script.

Abucus auto updates scripts except the clean, configure, build, install, and run functions.

It's just a simple git management system I created for cloning git projects and keeping them organized.

Zstd is required for archiving projects, you can change this in the template archive function and the check dependencies in the template and abucus. The template is the escaped string in abucus.
