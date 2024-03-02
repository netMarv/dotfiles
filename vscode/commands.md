For Unix-like shells (Zsh and Bash):

```bash
cat vs-extensions.txt | xargs -L1 code --install-extension
```

For Windows Command Prompt (CMD):

```cmd
for /F "tokens=*" %a in (vs-extensions.txt) do code --install-extension %a
```
