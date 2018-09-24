This repository contains a [Grafana][grafana] dashboard which shows graphs of the metrics collected from an application server using Microprofile Fault Tolerance 1.1.

* If you want to import this dashboard, [head over to the dashboard page on grafana.com][dashboard-page]
* If you want to report problems or suggestions, you can raise an issue on this repository

## Requirements

An application server which supports Microprofile Fault Tolerance 1.1. E.g.

* [Open Liberty][open-liberty]
* [Payara Server or Payara Micro][payara]

An application which uses the MicroProfile Fault Tolerance annotations.

## Instructions

* Deploy your app on the app server.
* Configure prometheus to collect metrics from the app server.
* Import this dashboard from [here][dashboard-page]
* At the top of the dashboard, there's a drop down which will be populated with the names of the annotated methods from your application.
    * If nothing appears here, first make sure you've called the annotated method and that the selected time range covers the execution. Then refresh the dashboard.

[grafana]: https://grafana.com/
[open-liberty]: https://openliberty.io
[payara]: https://www.payara.fish/
[dashboard-page]: https://grafana.com/dashboards/8022
