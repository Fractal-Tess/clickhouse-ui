# A CH-UI setup for Clickhouse


## Setup 

Setting up the webui for this repository goes as follows:

* Clone this repository:
```bash
git clone https://github.com/Fractal-Tess/clickhouse-ui.git
```

* Copy over the example `.env.example` file to `.env` and fill out the required fields:
```bash 
cp .env.example .env
```

* Run docker compose
```bash
docker compose up -d
```



> [!IMPORTANT]
> The webui service (CH-UI) uses your browser for the connection client.
>
> This means that the webui service (CH-UI) does not need to be part of the same network as the clickhouse instance.
> This also means that if you would like your webui to be able to connect, the clickhouse instance must be reachable by the host (browser) that the webui (CH-UI) is running on.
# clickhouse-ui
