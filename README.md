# activemq-artemis-operator-helmchart
ActiveMQ Artemis Operator Helm Chart

---
**_NOTES:_**

* Currently the Operator CRDs are stored in the templates directory and because of that when you uninstall the chart the CRDS are removed as well.
* This chart currently works only with [ArtemisCloud ActiveMQ Artemis Operator][1] version 0.20.1
* This chart currently only install the operator at namespace level

---
* ensure [helm tool][2] is installed and log in into your kubernetes cluster

* to install the chart:
```shell
helm install artemis-operator-chart . --values ./values.yaml
```

* to uninstall the chart:
```shell
helm uninstall artemis-operator-chart
```

[1]: https://github.com/artemiscloud/activemq-artemis-operator
[2]: https://helm.sh/docs/intro/install/