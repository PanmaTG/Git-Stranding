---
favicon: https://stackoverflow.com
---
**Link:** https://stackoverflow.com/questions/2845731/how-to-uncommit-my-last-commit-in-git

---
If you know you want to use `git reset`, it still depends what you mean by "uncommit". 

If all you want to do is **<span style="color:rgb(224, 222, 113)">undo the act of committing, leaving everything else intact</span>**, use:

```bash
git reset --soft HEAD^
```

If you want to **<span style="color:rgb(224, 222, 113)">undo the act of committing and everything you'd staged, but leave the work tree (your files) intact</span>**:

```bash
git reset HEAD^
```

And if you actually want to _completely_ undo it, _**throwing away all uncommitted changes, resetting everything to the previous commit**_ (as the original question asked):

```bash
git reset --hard HEAD^
```
