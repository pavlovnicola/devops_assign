# devops_assign

export blaa="key here"

curl -s -v https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT}/apis/batch/v1/namespaces/default/jobs/pi --cacert /var/run/secrets/kubernetes.io/serviceaccount/ca.crt --header "Authorization: Bearer $(echo $blaa)"

curl -s -vk https://${KUBERNETES_SERVICE_HOST}:${KUBERNETES_SERVICE_PORT}/apis/apps/v1/namespaces/default/deployments --header "Authorization: Bearer $(echo $blaa)"
