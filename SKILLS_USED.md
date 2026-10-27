# Tools used

- Python `requests`: polite link checker (HEAD with GET fallback, browser user agent, 6 concurrent, 3 tries with backoff; 403/429 counted as unverified, not dead)
- GitHub REST API (`GET /repos/{owner}/{repo}`): confirms each listed repo exists and catches renames, transfers and archived repos
- `git`: branch, commit, push
- `gh` CLI: pull request
- `gitleaks`: secret scan of the branch
