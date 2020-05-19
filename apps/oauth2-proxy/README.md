DESCRIPTION:
	A reverse proxy and static file server that provides authentication using 
	Providers (Google, GitHub, and others) to validate accounts by email, 
	domain or group.

	Github: https://github.com/oauth2-proxy/oauth2-proxy
	Docs: https://oauth2-proxy.github.io/oauth2-proxy/

USAGE:
	helm install oauth2-proxy airdb/oauth2-proxy --set service.client_id="apps.googleusercontent.com" \
		--set service.client_secret="secret" \
		--set service.cookie_secret="ht5SQYukAb" \
		--set service.cookie_domain="*"
	
	helm get notes oauth2-proxy
