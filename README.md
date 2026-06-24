# abucus
![ptyxis](https://github.com/knuxyl/abucus/blob/main/abucus.png?raw=true)

Shell script for managing, building, and running git projects

Like a package manager for git projects but lacks several features such as uninstalling a project from the system.

Currently rewriting it be to be posix compliant.

Can use a .conf file (optional) in the same directory as abucus named abucus.conf. Can change in script.

Abucus creates scripts for each project cloned that is independent or can be ran from the main abucus script.
This makes each project 100% self contained. If abucus disappears, all functionality will still be present in the project's script.

Abucus auto updates scripts except the clean, configure, build, install, dependencies, abucus dependencies, and run functions.

It's just a simple git management system I created for cloning git projects and keeping them organized.

Zstd is required for archiving projects, you can change this in the template archive function and the check dependencies in the template and abucus. The template is the escaped string in abucus.

I didn't create this for anyone else so it's probably not doing what you want. It creates a template using cmake/meson and ninja to configure and build a project. you just do

abucus c https://gitrepo.git

abucus nmb reponame
