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



# Azure creation app service for python

```
az group create -l <your-region> -n <your-resource-group>
```

```
az appservice plan create -g <your-resource-group> -n <your-appservice-plan> --is-linux --sku B1
```


```
az webapp create -g <your-resource-group> -p <your-appservice-plan> -n <your-appservice> --runtime "Python|3.6"
```

```
az webapp config set -g <your-resource-group> -n <your-appservice> --startup-file <your-startup-command-or-file>
```

ref: [HERE](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?toc=%2Fazure%2Fpython%2Ftoc.json&bc=%2Fazure%2Fpython%2Fbreadcrumb%2Ftoc.json&view=azure-devops)

