# Break-All-The-Things
Merge Conflict. I want to break things and then repair them. I expect to succeed at the first part but maybe not the second ...........


Specifically, I want to create a merge conflict.


---
## Setting up VS Code as your Git diff tool


You can set up VS Code as your tool to perform merge conflicts. To do so, you set it as your **difftoll** and your **merge tool** in your .gitconfig file on your computer. This can be done manually (byt finding your .gitconfi file on your computer), or by running osm ecomments in the command window/powershell.

```shell
git config --global diff.tool default-diff
git config --global difftool.vscode.cmd 'code --wait --diff "$LOCAL" "$REMOTE"'
git config --global difftool.prompt false

git config --global merge.tool vscode
git config --global mergertool.vscode.cmd 'code --wait -- resume  "$LOCAL" "$REMOTE"'
```
