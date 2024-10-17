## Progress (as of 10/17/24)

### Datasets
1. **Tox21**
2. **ClinTox**
3. **ToxCast**

Junction Trees were created for the majority of all three datasets.

### Done
- Run GNNs on all datasets.
- Insert lines of code that will create and update a spreadsheet with the desired values.
- Run `gSpan` on all raw datasets and junction tree datasets.
- Create dictionaries from `gSpan` outputs.
- Document, document, document

### To Do
-Fix KekulizeExceptions
-Add more accuracy measures learned in data science class

## Setting Up Git Access

1. Create an SSH key:
    ```bash
    ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
    ```
2. Grab the public key:
    ```bash
    cat ~/.ssh/id_rsa.pub
    ```
3. Copy the output and paste it into your GitHub settings.
4. Test the SSH connection:
    ```bash
    ssh -T git@github.com
    ```

You should see this message:
Hi username! You've successfully authenticated, but GitHub does not provide shell access.

#### To check the remote url
```bash
git remote -v
```
#### To change the ssh remote url
```bash
git remote set-url origin git@github.com:username/repo.git
```

#### Set up Git LFS for large file storage
TBA

#### If there's a lag due to LFS
```bash
git fetch origin
git reset --hard origin/main
```
-Fetchs remote changes without merging and sets head at most recent GitHub commit

#### To save local changes before reset (if GitHub repo was behind local and local changes should be kept when merging):
```bash
git stash
git reset --hard origin/main
git stash pop
```
