Setup

Prequisites
- Composer
- NodeJs
- Git
- SourceTree (optional)

* Install pre-requisites first before proceeding with the project setup.

1. Download nginx stack at https://bitnami.com/stack/nginx and install.
2. Key in localhost or 127.0.0.1 in your browser to check if nginx is up and running.


Cloning the project
1. Create a directory where you are going to store the project (e.g. D:\Projects).

2. Navigate into the root of your newly created directory and run git bash(right click -> git bash here)

3. Clone the project - https://github.com/iamreg/sampleapp.git

4. Once done, you should have now the directory structure like this - D:\Projects\sampleapp

5. Navigate to D:\Projects\sampleapp\apps using the windows console or git

6. Run composer update - this is to fetch all application dependencies


Setting up project to nginx server blocks(vhosts)

1. Update the correct project path in - D:\Projects\sampleapp\apps\conf\nginx-vhosts.conf

2. Open nginx app vhost config file - installationDirectory\nginxstack-1.12.2-2\nginx\conf\bitnami\bitnami-apps-vhosts.conf

3. Include the projects vhost config file path
	include "D:/Projects/sampleapp/apps/conf/nginx-vhosts.conf";
	
4. Restart nginx