# Deploy notes
- Live URL: https://nchandler02-sudo.github.io/lecture-app/
- Repo: https://github.com/nchandler02-sudo/lecture-app (public), GitHub Pages from `main` branch, root `/`.
## Update
    cd /workspace/lecture-app
    cp /path/to/new/index.html index.html   # replace with production app
    git add -A && git commit -m "Production app" && git push
Pages rebuilds automatically in about 1 minute. Check: `gh api repos/nchandler02-sudo/lecture-app/pages/builds/latest --jq .status`
then `curl -sI https://nchandler02-sudo.github.io/lecture-app/`.
