# dictybase-postgres-template
A template source repository for creating customized postgresql [docker](http://docker.io)
image.

## Usage
- Clone this repository.  
- Rename three template files and edit their content accordingly, preferably the commented sections.
 - `README.template` __-->__  `README.md`. It should overwrite this file though.
 - `01_create_users.template` __-->__  `01_create_users.sh`. Make sure you make
   it executable(chmod). You could of course add more script file as necessary.
   Those script files will be copied to the appropriate folder to be run during
   startup.
 - `Dockerfile.template` __-->__ `Dockerfile`. Change the base image if needed.
 - Modify configuration files(.conf) as necessary.
 - Finally create the docker image.
