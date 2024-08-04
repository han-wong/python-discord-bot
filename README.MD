# Discord Bot

## Virtual environment
PowerShell
```ps
python -m venv .venv
.venv\Scripts\Activate.ps1
```

## Install
PowerShell
```ps
pip install -r requirements.txt
```

## Bug
* Go to: .venv\Lib\site-packages\interactions\client\smart_cache.py", line 201, in GlobalCache
* Change: discord_typings.resources.guild.GuildMemberData
* To: discord_typings.GuildMemberData

## Change environment variables
* Copy .env.sample to .env and fill in the variables

## Develop
PowerShell
```ps
pymon main.py -w ./extensions
```

## Production
PowerShell
```ps
python main.py
```