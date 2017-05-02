Art/Earth/Tech website: http://artearthtech.com/

Central git repo is on gitlab:

https://gitlab.com/artearthtech/artearthtech.com


## Site Architecture

TODO


## Technical Stuff

* The source is managed in git.
* The website is statically built using hugo.

To work on the website:

* Install hugo (requires '_go_')
* Install git lfs and pull git large files
* Run hugo:

  `hugo server`

### Deployment

We deploy it using gitlab pipelines -- see .gitlab-ci.yml

### Assets

All assets for the site are stored in [this drive folder](https://drive.google.com/drive/u/1/folders/0B4VpjxPkN_XccDdOOGNVZlo1VXM).

We use reduced (pixels and file size) versions of the images to increase pages' loading speed. All reduced images have appendix with `W x H` in their names.
