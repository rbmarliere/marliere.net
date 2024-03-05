## [marliere.net](https://marliere.net)

My personal site, generated with [Hugo](https://gohugo.io).

---

.git/hooks/pre-commit:
```bash
#!/bin/sh

rm -rf public/
hugo
git add --all public resources/_gen
```

post-clone:
```bash
~/.local/share/nvim/mason/bin/vale sync
```
