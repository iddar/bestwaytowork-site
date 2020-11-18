# bestwaytowork-site

site for my personal site bestwayto.work

```sh
# Setup
git config git-ftp.url $FTP_URL # example "ftp://ftp.example.net:21/public_html"
git config git-ftp.user $FTP_USER
git config git-ftp.password $FTP_PASS

# Upload all files
git ftp init

# Or if the files are already there
git ftp catchup

# Work and deploy
echo "new content" >> index.txt
git commit index.txt -m "Add new content"
git ftp push
# 1 file to sync:
# [1 of 1] Buffered for upload 'index.txt'.
# Uploading ...
# Last deployment changed to ded01b27e5c785fb251150805308d3d0f8117387.
```
