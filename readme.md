
Use git reset --hard to move back to the first commit and take a screenshot:

```bash
git reset --hard HEAD~1
```

![image](https://github.com/user-attachments/assets/b2d1b98e-ff4d-4968-aae5-81931d239e1e)
![image](https://github.com/user-attachments/assets/49a9e88e-4f05-47ad-aea2-8750c1f190bb)

Use git reflog to find the previous state (second commit), reset back to it, and take screenshots from reflog and after resetting:

```bash
git reflog
git reset --hard HEAD@{1}
```
![image](https://github.com/user-attachments/assets/892e2b58-e29e-4d04-a611-00bd2b8caf33)


Switch again to `alpha` and visualize the log graph:

```bash
git log --oneline --decorate --all --graph
```

![image](https://github.com/user-attachments/assets/48bf2dde-7b3b-4815-9b2b-9c3a14fb54f7)

Rebase develop onto alpha:
```bash
git rebase develop
```

![image](https://github.com/user-attachments/assets/4838b37b-d944-4a95-8c47-5055bf635133)

