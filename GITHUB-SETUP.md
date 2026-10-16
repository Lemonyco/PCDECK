# GitHub setup — public showcase repository

Recommended repository name: `PCDeck`

1. Create a **Public** GitHub repository.
2. Extract this folder and run:

```powershell
git init
git add .
git commit -m "Launch PCDeck public showcase"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/PCDeck.git
git push -u origin main
```

3. In GitHub repository settings:
   - Enable Issues.
   - Enable Discussions when you are ready for a community.
   - Enable private vulnerability reporting.
   - Add topics such as `windows`, `tablet`, `automation`, `productivity`, `remote-control`, `python`, and `javascript`.
4. Add the 30-second demo video/GIF and clean screenshots before announcing the repo publicly.
5. Publish paid/signed builds through GitHub Releases; keep the commercial source private.
