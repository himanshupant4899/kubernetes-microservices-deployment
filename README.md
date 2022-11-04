# kubernetes-microservices-deployment

The project depicts the deployment of a sample microservices application using helm charts.

### To create a helm chart: ```helm create chart_name```
> helm create microservice

### To validate the file locally: ```helm template -f file_to_ovveride_default_values chart_name```
> helm template -f values/email-service-value.yaml charts/microservice

### To examine a chart for possible issues: ```helm lint -f file_to_ovveride_default_values chart_name```
> helm lint -f values/email-service-value.yaml charts/microservice

### For dry run:
> helm install --dry-run -f values/email-service-value.yaml charts/microservice

### To install the components created execute the following command: ```helm install -f file_to_ovveride_default_values release_name```
> helm install -f values/email-service-values.yaml emailservice

## OR alternatively using a helmfile.
