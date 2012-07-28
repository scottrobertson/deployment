# Deployment Script

With this script, you can deploy a website using nothing more than SSH.

# Intructions

 - `Add this folder to your PATH`
 - `Setup SSH access to your server`
 - `Configure the .deploy file`
 - `Configure the .deploy_ignore file`
 - `Deploy!`

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

 - `.deploy_success`
 - `.deploy_before`