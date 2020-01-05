# othello_bot
othello_bot for univ.

### Note
If you use this service in systemd, You need to change .api_token relative path in AuthCheck.py to absolute path.

### systemd setting for non-root environment

```
mkdir -p .config/systemd/user/
cp othello.service .config/systemd/user/
systemctl --user daemon-reload
systemctl --user enable othello.service
systemctl --user start othello.service
```

### Directory structure

```
+ OthelloArenaPython/
|-- AuthCheck.py
|-- OthelloAction.py
|-- OthelloLogic.py
|-- Play.py
|-- TestPlay.py
|-- main.py <- SET HERE
```
