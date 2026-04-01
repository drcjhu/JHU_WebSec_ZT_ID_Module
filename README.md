
# JHU WebSec Course Zero Trust Identity Management Module Assignment Config Files

This repository contains the config files for the assignment.

Use these files to build the lab environment in your Linux sandbox so you can focus on the real goal of the assignment: applying Zero Trust and identity management principles to a web application, then evaluating the result using AAA and CI4A.

## Files in this repository

- `JHUWebSec_IDZT_files.zip`  
  Zip archive containing all assignment files.

These are the files in the Zip:
- `docker-compose.yml`  
  Starter Docker Compose file for the lab stack.

- `configuration.yml`  
  Main Authelia configuration file.

- `users_database.yml`  
  Local user database for the lab.

- `admin_adv.config`  
  Reverse proxy configuration used to protect the admin path with the identity layer.

- `ghostBlock.config`  
  Reverse proxy configuration used to block direct access to the `/ghost` path.

## How to get the files in your Linux sandbox

You may either download the zip file or download the individual files.

### Option 1, download the zip file
Download `JHUWebSec_IDZT_files.zip` into your Linux sandbox, then unzip it.

Example in bash:
$ mkdir -p ~/IDZT
$ cd ~/IDZT
$ wget https://github.com/drcjhu/JHU_WebSec_ZT_ID_Module/blob/main/JHUWebSec_IDZT_files.zip
$ unzip JHUWebSec_IDZT_files.zip

If your instructions place files in slightly different locations, follow the assignment guidance. The main goal is to keep the environment organized and easy to troubleshoot.

~/Mod11_IDZT/
├── docker-compose.yml
├── admin_adv.config
├── ghostBlock.config
├── authelia/
│   └── config/
│       ├── configuration.yml
│       └── users_database.yml
