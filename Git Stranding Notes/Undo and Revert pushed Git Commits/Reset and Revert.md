---
favicon: https://github.com
---
**Link:** https://www.theserverside.com/video/Undo-and-revert-pushed-Git-commits

---

# Undo and revert pushed Git commits

## git reset
1) Check git commits and their hashes first
	```bash
	git log --oneline
	```

2) Get the hash of the previous commit, before the bad one. In this example, let's say the `9b029ad` is the bad one. Therefore, we get the previous one, which is `ccb9118`
	
	![[Git Reset img1.png]]

 3) Use `git reset --hard <hash commit>` command
	```bash
	git reset --hard ccb9118
	```

4) It will automatically **put you in that previous commit.**

5) **To delete it from the GitHub repo**, use `git push --force` command
	```bash
	git push --force
	```

## git revert