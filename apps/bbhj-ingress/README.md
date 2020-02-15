DESCRIPTION:
	bbhj-ingress dependence on Tencent Load Balance and SSL Cert.

REPO:
	helm repo add airdb https://www.airdb.com/helm/
	helm repo update
	helm search repo airdb

USAGE:
	helm install bbhj-ingress airdb/bbhj-ingress --set service.qcloud_lb=$existLbId

	helm install bbhj-ingress airdb/bbhj-ingress --set service.qcloud_cert_id=$cert_id
