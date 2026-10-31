# Linux File Permissions

An educational project from the Google Cybersecurity Certificate demonstrating how Linux commands can be used to review and update file and directory permissions.

## Project overview

In this exercise, I reviewed permissions in a simulated research-team projects directory and adjusted access to better follow the principle of least privilege. The write-up explains how `ls -la` displays permissions and hidden files, and how `chmod` changes access.

## Commands and changes

- `ls -la` displayed the directory contents, including the hidden file `.project_x.txt`, along with permissions, owners, and groups.
- `chmod o-w project_k.txt` removed write access for others from `project_k.txt`. The permission string changed from `-rw-rw-rw-` to `-rw-rw-r--`.
- `chmod u-w,g+r,g-w .project_x.txt` removed write access and gave the group read access to the archived hidden file. Its resulting permissions were `-r--r-----`.
- `chmod g-x drafts` removed the group’s execute/search permission from `drafts`. Its resulting permissions were `drwx------`, leaving access to the directory with its owner, `researcher2`.

## Skills demonstrated

- Inspecting Linux file and directory permissions with `ls -la`
- Interpreting owner, group, and other permission bits
- Using symbolic `chmod` arguments to change access
- Recognizing hidden files and applying least privilege

## Coursework document

[View the completed File permissions in Linux activity](File%20permissions%20in%20Linux.pdf)

This project documents a simulated coursework exercise; it does not describe changes made to a live organization’s file system.
