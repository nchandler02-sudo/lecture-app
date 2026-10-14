# Deploy notes
- Live URL (audience / final app): https://nchandler02-sudo.github.io/lecture-app/
- Speaker Mad Lib builder: https://nchandler02-sudo.github.io/lecture-app/builder.html
- Kahoot import file: https://nchandler02-sudo.github.io/lecture-app/kahoot-madlib.xlsx
- Repo: https://github.com/nchandler02-sudo/lecture-app (public), GitHub Pages from `main` branch, root `/`.

## Update the live app during the talk
    cd /workspace/lecture-app
    cp /path/to/new/index.html index.html
    git add index.html && git commit -m "Live app" && git push
Pages rebuilds in about 1 minute. Check: `gh api repos/nchandler02-sudo/lecture-app/pages/builds/latest --jq .status`
then `curl -sI https://nchandler02-sudo.github.io/lecture-app/`.
