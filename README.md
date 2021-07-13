# PingMonitor for InfluxDB v2

### Configuration (Caution : CASE SENSITIVE): 
```
{
	"hosts" : [
		"1.1.1.1",
		"google.com",
		"8.8.8.8",
		"4.2.2.4",
		"koorosh.dev",
		"blog.koorosh.dev"
	],
	"influx" : {
		"url" :"http://127.0.0.1:8086",
		"secret" : "6cXZN5nqN63kO3fSP9dE5M4lQXN08bvPK0SqCZqPGIeamkH2ejgNWhdafxzIyij-nohj3g94YJ_gvW_20MKWFg==",
		"org": "local",
		"bucket" : "Ping"
	}
}
```
<b>hosts</b> : list of hosts that you want to monitor  
<b>influx</b> :
- url : http address of your Influx Instance
- secret : Influx Token with write permission
- org : organization 
- bucket : database name


### How-to Run 
java -jar PingMonitor.jar -c config.json

### Depnds on :
<a href="https://commons.apache.org/proper/commons-cli">Apache Commons CLI</a>  
<a href="https://github.com/google/gson">GSON</a>  