# QMantis: Observability and monitoring for GraphQL APIs

## How to set up QMantis

### QMantis infrastructure
* In the root folder of your GraphQL API, where you imported `qmantis-server-express`, you'll need to:
  1. Run the Docker daemon
  2. Clone this `qmantis-compose` directory
  3. `cd` into `qmantis-compose` 
  4. Create an .env file that includes `POSTGRES_USER` and `POSTGRES_PASSWORD`
  5. Execute `docker-compose up`

* To visualize your metrics and traces, access Grafana at port 3000.
* When you first access Grafana, you will be prompted to enter a username and password. Type in `admin` for the username and `admin` for the password. You will then be asked to change the password.
* After logging in, on the left side of the screen, click on Dashboards > Browse, then click on the 'qmantis' dashboard.
* In this dashboard, you will see the panels:
  * Request Rate
  * Request Latency
  * All Traces
  * Error Rate
  * Error Traces
