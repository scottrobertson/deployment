# Deployment Script

With this script, you can deploy a website using nothing more than SSH and rsync. All you need to do is run the command "deploy master" or "deploy beta" or anything you wish, and the script will take care of the rest.

# Intructions

 - `Add this folder to your PATH`
 - `Setup SSH access to your server`
 - `Configure the .deploy file`
 - `Deploy!`

# Requirements

 - `SSH`
 - `rsync (If you are using Windows, download Cygwin and install rsync)`

## Example .deploy file

 - `master user@example.com /home/example.com/public_html true`
 - `beta user@example.com /home/example.com/public_html/beta true`

## Example .deploy_ignore file

 - `.git`
 - `/tmp`

## Example deploy command file

 - `deploy beta`


---------

### Deploy File Config

 - `branch sshlogin path fixpermissions`

### Optional Files

 - `.deploy_success (This is run on the server once the deployment has finished. Flushing the Cache maybe?)`
 - `.deploy_before (This will be run before files are syned to server. Compress CSS maybe?)`
 - `.deploy_ignore (All the files/folders in this file will be ignore. One per line)`
