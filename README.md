# tapyrus_playground

気軽に Docker で Tapyrus testnet に接続しながら tapyrusrb をいじれるレポジトリ

## Setup

Require: Docker compose v2 ~

```bash
# Create containers
$ make docker/up

# Show logs
$ make docker/logs

# Wait for initial block downloads

# Run irb
$ make ruby/irb
irb> require 'tapyrus'
=> true
```

> **Note**
> When connect tapyrus node, specify HOST as "tapyrusd".

## Make commands

```bash
# Start containers
$ make docker/start

# Stop containers
$ make docker/stop

# Remove containers (also volumes will removed)
$ make docker/down

# Show logs
$ make docker/logs

# Run irb
$ make ruby/irb
irb> require 'tapyrus'
=> true
```
