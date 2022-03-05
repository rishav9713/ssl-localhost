# ssl-localhost



<VirtualHost *:80>
	DocumentRoot "F:\xampp\htdocs"
	ServerName sites.local
	ServiceAlias *.sites.local
	SSLEngine on
	SSLCertificateFile "crt/sites.local/server.crt"
	SSLCertificateKeyFile "crt/sites.local/server.key"
	
</VirtualHost>


# access-everywhere

ngrok http 82 -host-header="localhost:82"
