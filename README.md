
# Deployment

Deploying the site is simple.

### When you've made all the necessary changes, verify them:

    gs

**Output should something like the following:**

    Jacob:rudderandoar jacobthomas$ gs
    # On branch: master  |  [*] => $e*
    #
    ➤ Changes not staged for commit
    #
    #       modified: [1] config.toml
    #
    ➤ Untracked files
    #
    #      untracked: [2] README.md
    #      untracked: [3] static/img/about/
    #
    Jacob:rudderandoar jacobthomas$
    

### Then, add all changes to git with `ga 1-X`, x being the number of files that have been changed:

    Jacob:rudderandoar jacobthomas$ ga 1-3
    # Added '/Users/jacobthomas/Desktop/rudderandoar/config.toml'
    # Added '/Users/jacobthomas/Desktop/rudderandoar/README.md'
    # Added '/Users/jacobthomas/Desktop/rudderandoar/static/img/about/'
    #
    # On branch: master  |  [*] => $e*
    #
    ➤ Changes to be committed
    #
    #       new file: [1] README.md
    #       modified: [2] config.toml
    #       new file: [3] static/img/about/smith_wedding.jpg
    #
    Jacob:rudderandoar jacobthomas$
    

### Commit your changes to the `master` branch and add a commit message with `gc -m "Message"`

    Jacob:rudderandoar jacobthomas$ gc -m "Adds smith wedding and about section"
    [master ff5a30b] Adds smith wedding and about section
     3 files changed, 16 insertions(+), 5 deletions(-)
     create mode 100644 README.md
     create mode 100755 static/img/about/smith_wedding.jpg
    Jacob:rudderandoar jacobthomas$
    
### Finally, push the changes to the `master` branch of the repository with `gps origin master`
