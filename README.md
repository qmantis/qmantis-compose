# QMantis: Observability and monitoring for GraphQL APIs

## How to set up QMantis

* In the server that'll host QMantis, where you imported either `qmantis-server-js` or `qmantis-server-express`, you'll need to:
  1. Run the Docker daemon
  2. Clone this `qmantis-compose` directory
  3. `cd` into `qmantis-compose` and execute `docker-compose up`

* To visualize your metrics and traces, visit Grafana at port 3000.
* When you first visit Grafana, you will be prompted to enter a username and password. Type in `admin` for the username and `admin` for the password. You will then be asked to change the password.
* After logging in, on the left side of the screen, click on Dashboards > Browse, then click on the 'qmantis' dashboard.
* In this dashboard, you will see the panels:
  * Request Rate
  * Request Latency
  * All Traces
  * Error Rate
  * Error Traces
