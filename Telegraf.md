# Global Agent Configuration
[agent]
  hostname = "mynode-mainnet" # set this to a name you want to identify your node in the grafana dashboard
  flush_interval = "15s"
  interval = "15s"

# Input Plugins
[[inputs.cpu]]
    percpu = true
    totalcpu = true
    collect_cpu_time = false
    report_active = false
[[inputs.disk]]
    ignore_fs = ["devtmpfs", "devfs"]
[[inputs.diskio]]
[[inputs.mem]]
[[inputs.net]]
[[inputs.system]]
[[inputs.swap]]
[[inputs.netstat]]
[[inputs.processes]]
[[inputs.kernel]]
[[inputs.diskio]]

# Output Plugin InfluxDB
[[outputs.influxdb]]
  database = "metricsdb"
  urls = [ "http://metrics.stakeconomy.com:8086" ] # keep this to send all your metrics to the community dashboard otherwise use http://yourownmonitoringnode:8086
  username = "metrics" # keep both values if you use the community dashboard
  password = "password"

[[inputs.exec]]
  commands = ["sudo su -c /home/solana/solanamonitoring/monitor.sh -s /bin/bash solana"] # change home and username to the useraccount your validator runs at
  interval = "5m"
  timeout = "1m"
  data_format = "influx"
  data_type = "integer"
