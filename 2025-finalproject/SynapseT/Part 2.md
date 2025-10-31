# 二：

1. ：
   
   ```
   git reset HEA后git checkout -- .
   ```
   
   ***或者***
   
   ```
   git stash push --include-untracked
   ```

<img src="./Screenshot from 2025-10-31 22-36-05.png" title="" alt="示例" width="652">
![示例](./Screenshot from 2025-10-31 22-36-55.png)

---

2. ：

```
不修改历史的方式：git reset --soft HEAD~1
修改历史的方式：git reset --soft HEAD~1
```

![eg](./Screenshot from 2025-10-31 22-37-15.png)

---

3. ：
   
   ```
   git checkout main
   git cherry-pick <commit-hash1> <commit-hash2>
   git cherry-pick <start-commit>..<end-commit>
   ```
   
   ***或者***
   
   ```
      git checkout feature-branch
   git format-patch main --stdout > feature.patch
   git checkout main
   git apply feature.patch
   ```
   
   ![eg](./Screenshot from 2025-10-31 22-37-30.png)
