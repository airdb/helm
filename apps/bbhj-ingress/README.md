DESCRIPTION:
	bbhj-ingress dependence on Tencent Load Balance and SSL Cert.

USAGE:
	helm install chart airdb/mychat --dry-run --debug 

	helm install bbhj-ingress airdb/bbhj-ingress --set service.qcloud_lb=$existLbId

	helm install bbhj-ingress airdb/bbhj-ingress --set service.qcloud_cert_id=$cert_id
