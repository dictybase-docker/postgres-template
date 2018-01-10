# dictybase-postgres-template
A template source repository for creating customized postgresql [docker](http://docker.io)
image.

## Usage
- Clone this repository.  
- Rename three template files and edit their content accordingly, preferably the commented sections.
  - __`README.template` -->  `README.md`__. It should overwrite this file though.
  - __`01_create_users.template` -->  `01_create_users.sh`__. Make sure you make
   it executable(chmod). You could of course add more script file as necessary.
   Those script files will be copied to the appropriate folder to be run during
   startup.
  - __`Dockerfile.template` --> `Dockerfile`__. Change the base image if needed.
  - Modify configuration files(.conf) as necessary.
  - Finally create the docker image.
  - To push it to a remote repository, make sure to change the url.
