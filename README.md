
	      ____                  __          ____
	     / __ \____  _____ ____/ /_  ____  / / /_
	    / /_/ / __ `/ ___/ ___/ __ \/ __ \/ / __/
	   / ____/ /_/ (__  |__  ) /_/ / /_/ / / /_
	  /_/    \__,_/____/____/_,___/\____/_/\__/

	The open source password manager for teams
	Copyright (c) 2025 Passbolt SA
	https://www.passbolt.com

## Variables

### Database configuration

|Name|Default value|Allowed values|Mandatory?|Description|
|-|-|-|-|-|
|`database_configuration.dbname`|`passbolt_db`|String|❌|The name of the Passbolt database.|
|`database_configuration.username`|`passbolt_db_user`|String|❌|The name of the Passbolt database user.|
|`database_configuration.host`|`null`|String representing an IP or a FQDN|❌|The database host. Anything other than `null` will be treated as an external database (thus disabling database installation and creation)|
|`database_configuration.password`||String|✅|The password for the Passbolt database user.|
|`nginx_configuration.fqdn`|`passbolt.local`|String|❌|The Fully-Qualified Domain Name for your Passbolt server, without any `http` or `https` schema.|
|`nginx_configuration.certbot_email`||String|❌|The e-mail to provide to certbot for certificates renewal and other notifications. *By providing this e-mail, this `ansible` playbook will accept the TOS.|
|`nginx_configuration.manual_certificate.fullchain_certificate`||String|❌|The fullchain certificate content when using manually generated certificates.|
|`nginx_configuration.manual_certificate.private_key`||String|❌|The private key content when using manually generated certificates.|
