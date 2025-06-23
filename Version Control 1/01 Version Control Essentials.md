---
tags:
  - instructor-manual
  - version-control
  - evergreen
  - VC1
last_modified: 2025-04-21
---
## Common Misconceptions

| Misconception                                     | Explanation                                                                                                                                                                                                                                                                                                        |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Committing frequently clutters the commit history | Frequent commits improve traceability and ease of debugging. Encourage small, logical commits with clear messages. See example: [[#Frequent‑Commits‑Example]].<br>小さな論理的なコミットと明確なメッセージは、履歴の追跡性とデバッグを容易にします。例は [[#Frequent‑Commits‑Example\|頻繁なコミットの例]] を参照してください。                                                  |
| Branches are just copies or folders of the repo   | \ Branches are lightweight pointers to commits, not full copies. They enable parallel work without duplication. See example: [[#Branch‑Pointer‑Example\|Branch Pointer Example]].<br>ブランチはコミットへの軽量ポインタであり、重複なく並行作業を可能にします。例は [[#Branch‑Pointer‑Example\|ブランチポインタの例]] を参照してください。                                    |
| Force‑pushing is a quick fix for mistakes         | `git push --force` can overwrite remote history and affect collaborators. Use `--force-with-lease` or revert commits instead. See example: [[#Force‑Push‑Dangers\|Force‑Push Dangers]].<br>`git push --force` は共同作業者に影響を与える可能性があります。`--force-with-lease` を使いましょう。例は [[#Force‑Push‑Dangers\|強制プッシュの危険性]] を参照してください。 |
| Rebasing public branches is safe                  |  Rebasing rewrites history; avoid on shared branches to prevent confusion. Use on local or feature branches before sharing. See example: [[#Rebase‑Best‑Practices\|Rebase Best Practices]].<br> 共有ブランチでのリベースは混乱を招く可能性があります。共有前のローカルブランチで使用しましょう。例は [[#Rebase‑Best‑Practices\|リベースのベストプラクティス]] を参照してください。           |

## Example Walk‑Throughs  

### Frequent‑Commits‑Example 
**(What to demonstrate in class)**  
1. Create a tiny text file (`notes.txt`).  
2. Add one line, commit with message `feat: add header`.  
3. Add a second line, commit `feat: add introduction`.  
4. Run `git log --oneline --graph` and show how each logical step is documented.  

**授業での実演ポイント）**  
1. 小さな `notes.txt` を作成。  
2. 1 行目を追加して `feat: add header` でコミット。  
3. 2 行目を追加して `feat: add introduction` でコミット。  
4. `git log --oneline --graph` を実行し、各ステップが履歴に残る様子を示す。  

---

### Branch‑Pointer‑Example 
 
```bash
git init branch-demo && cd branch-demo
echo "v1" > readme.md && git add . && git commit -m "v1"
git branch feature-a
git checkout feature-a
echo "feature work" >> readme.md && git commit -am "feat: work on A"
````

Show `git log --oneline --decorate --graph` – learners see that _feature‑a_ is simply another pointer diverging from _main_.
 
`git log --oneline --decorate --graph` を表示して、_feature‑a_ がコピーではなくコミットへのポインタであることを視覚的に伝える。

---

### Force‑Push‑Dangers 

1. Clone a shared repo, make a commit, and `push`.
    
2. On another clone, amend the same commit and `git push --force`.
    
3. Return to the first clone, pull, and show the _divergent history_ error.
    
4. Repeat using `--force-with-lease` to highlight its safety check.
    

5. 共有リポジトリを複製し、コミットして `push`。
    
6. 別の複製で同じコミットを修正し `git push --force`。
    
7. 最初の複製で `git pull` すると履歴が食い違うエラーを確認。
    
8. `--force-with-lease` の再実演で安全性を比較。

### Rebase‑Best‑Practices 

```bash
# local feature branch
git checkout -b feature-b
# work...
git commit -am "feat: finish B"

# BEFORE sharing, update history neatly
git fetch origin
git rebase origin/main
```

Explain that rebasing _before_ pushing keeps the public history linear; rebasing _after_ others pull causes headaches.
  
プッシュ前のリベースで履歴を整理するのは良い慣行だが、既に共有されたブランチをリベースすると履歴が書き換わり、他の開発者が混乱することを説明。