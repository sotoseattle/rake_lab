#RAKE LAB

Some experiments involving Rake to learn the DSL and derive some useful value.

### Ideas

1. 'rake blog': A task to create an environment in tmux for working on my site.
    - editor: 1 window with vim open to public posts
    - server: another at the root that has launched the website
    - shell: another at the root with the last 10 posts modified listed
2. 'rake cleanex': A task to remove the annoying latex auxiliary files
    - only removes files inside the dir where the rake call is made
    - removes '*.log' and '*.aux'

