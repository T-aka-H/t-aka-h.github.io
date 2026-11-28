# holdline-support

Static support / privacy pages for the Holdline iOS app, served via GitHub Pages.

URLs:
- Support: https://taka-ku.github.io/holdline-support/
- Privacy: https://taka-ku.github.io/holdline-support/privacy.html

## Setup (one time)

```sh
cd ~/app_dev/holdline-support
git init -b main
git add -A
git commit -m "Initial support page"
gh repo create taka-ku/holdline-support --public --source=. --push
# GH Pages を main / root から有効化
gh api -X POST /repos/taka-ku/holdline-support/pages -f source[branch]=main -f source[path]=/
```

`gh` (GitHub CLI) が無ければブラウザから手動で作成 + push でも OK。
