# Python/Flask sample for Visual Studio Code

# Mac/Linux (bash)

```bash
sudo apt-get install python3-venv  # If needed
python3 -m venv .env
source .env/bin/activate
pip install -r requirements.txt
export set FLASK_APP=hello_app.webapp
python3 -m flask run
```


# Windows (powershell)

```
py -3 -m venv .env
.env\scripts\activate
pip install -r requirements.txt
$env:FLASK_APP = "hello_app.webapp"
python -m flask run
```


