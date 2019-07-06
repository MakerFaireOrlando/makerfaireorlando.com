#Creating a local build / test environment

We will use the Bitnami Wordpress stack since we use Bitnami Wordpress on makerfaireorlando.com

##Steps
1) Get the bitnami wordpress stack installer for your OS
2) Install & start the server
3) Login (click the bitnami logo in the bottom right corner for credentials)
4) Install the updraft plugin (downloaded from website, not the wordpress hosted on). You will need Updraft credentials for this
5) Authenticate the plugin and authorize the site and the migrator utility. You will need Updraft credentials for this
6) Move all the backup files to this new instance. You can use filesystem, or drag & drop them to the updraft page on the test site once the plugin is installed
7) Install git (`apt update` & `apt install git` - you may need sudo)


##Troubleshooting

###File access & editing
If you can't edit files in the filesystem (with terminal / ssh or when mounted using the mount button), you may hit a problem that Ian encountered. 
Use the Bitnami app to open a terminal session. If you are connected as root, then `su bitnami` and `cd ~'
The system will then prompt you for a password. For Ian, everything worked after that (but I need to do this user change every time)



