# Grafana setup
## Setup steps
[official install instructions](https://grafana.com/tutorials/install-grafana-on-raspberry-pi/)

### Install
I followed the steps from the official instructions pretty straightforward, copied here in case they change...

1. Add the APT key used to authenticate packages:

>wget -q -O - https://packages.grafana.com/gpg.key | sudo apt-key add -

2. Add Grafana APT repo:

>echo "deb https://packages.grafana.com/oss/deb stable main" | sudo tee -a /etc/apt/sources.list.d/grafana.list

3. Install Grafana:

> sudo apt-get update
>
> sudo apt-get install -y grafana

4. enable in systemctl

> sudo /bin/systemctl enable grafana-server

5. Start Grafana

> sudo /bin/systemctl start grafana-server

it will start up on [port 3000](http://localhost:3000)