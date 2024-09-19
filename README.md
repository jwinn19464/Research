## Progress (as of 9/19/24)

### Datasets
1. **Tox21**
2. **ClinTox**
3. **ToxCast**

Junction Trees were created for the majority of all three datasets.

### To Do
- Run GNNs on all datasets.
- Insert lines of code that will create and update a spreadsheet with the desired values.
- Run `gSpan` on all raw datasets and junction tree datasets.
- Create dictionaries from `gSpan` outputs.

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
`git remote set-url origin git@github.com:username/repo.git`
