Art / Earth / Tech website: http://artearthtech.com/

## Content Team Guide

### Image Resizing

We have created an `imgresize` shortcode which will automatically do image resizing for you.

Suppose you have an image in `images` directory named:

`sitting-room.jpg`

Rather than embedding this in your post by doing:

```
<img src="/images/sitting-room.jpg" />
```

You would do:

```
{{< imgresize src="sitting-room.jpg" size="800x" >}}
```

Where `800x` means width of 800px. If you want height of 800px you would do `x800`. For more information on this option see image resizing in hugo see: https://gohugo.io/content-management/image-processing/

## Assets

All assets for the site are stored in [this drive folder](https://drive.google.com/drive/u/1/folders/0B4VpjxPkN_XccDdOOGNVZlo1VXM).

We use reduced (pixels and file size) versions of the images to increase pages' loading speed. All reduced images have appendix with `W x H` in their names.

---

## Technical Stuff

This website is a static website.

* The source is managed in git.
  * The central git repo is on gitlab: https://gitlab.com/artearthtech/artearthtech.com
* The website is statically built using [hugo][].

[hugo]: https://gohugo.io/

### To work on the website locally

* Install [hugo]
* Install git lfs and pull git large files
* git clone the repo:

  `git clone https://gitlab.com/artearthtech/artearthtech.com`
* Run hugo:

  `hugo server`

### Extras

To build the CSS from the SASS:

1. Install sass (e.g. `brew install sass`)
2. Run:

   `sass --watch static/scss:static/css`


### Deploying the website

We deploy the website live using gitlab pipelines.

Just `git push` and the new version of the site will go live.

If you want to learn more about how this happens see `.gitlab-ci.yml` file.


