# Preface
Working through John Savill's DevOps Master Class and some additional material via Microsoft Learn

# Notes
### Foundation
- Things like patching OS and whatnot don't really bring value to the org, hence why they tend to be avoided in DevOps
- SCRUM always contains **only** pull motions
- SCRUM contains sprints, which are a fixed duration of work
- SCRUM can use kanban boards, but they assign points to each item of work
    - Instead of WIP limits, they use point limits
- Generally, team sizes do not pass what you can feed with 2 pizzas
- Kanban is always in motion
- Pull when you have space
- Self-service is key to agility
### Mastering Git
- Centralized source control is generally not used anymore. 
    - This requires someone to check out files in order to work on it, creating a lock on those files
- Git is distributed, since all devs have a copy of all files
    - You sync with the remote origin
- `git config` allows you to change some attributes, like `user.name`
- You can change the default branch name by the following:
    - `git config --global init.defaultBranch main`
- All objects in git end up stored as a blob
- All blobs have a hash (sha1)
- This hash is used to find changes
- A tree has a file name, and uses a file pointer to point to the blob
- A commit is a snapshot of the entire repo which points to a certain tree, and contains additional metadata like author and date
- `git init` created a `.git` subfolder
    - this has an `objects` folder
- 