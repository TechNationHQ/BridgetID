# bridgetID
The BridgetID service will be responsible for managing unique IDs for all services and users within the network,
while the Chiral Gateway will handle routing requests between different micro services and ensuring authentication and authorisation for incoming requests.
# ▹ Run using docker #
> [!NOTE]  
> For start make sure you have docker installed on your machine.
```bash
sh scripts/run.sh
```
or
``` bash
docker-compose up --build -d
```
# ▹ Installation #
> [!NOTE]  
> For start make sure you have python and redis and mongodb installed on your machine.
``` Bash
git clone https://github.com/x
cd x
python3 -m venv .venv
source .venv/bin/activate
pip3 install -r requirements.txt
```   
Rename ```sample.env -> .env``` and don't forget to change the settings inside.

# ▹ Run #
``` Bash
source .venv/bin/activate
uvicorn app.main:app --host 0.0.0.0 --port 8080
```

## License

This project is licensed under the terms of the None license.