# RSE Midlands Website

The website can be found at [rse-midlands.github.io](https://rse-midlands.github.io). The website is built using [hugo](https://gohugo.io/).

## Workflow

The page is built and deployed when a commit to main is made. The deployment script can be found [here](https://github.com/RSE-Midlands/rse-midlands.github.io/blob/main/.github/workflows/build_and_deploy.yml) and details of deployments are found [here](https://github.com/RSE-Midlands/rse-midlands.github.io/actions).

If you wish to generate the site locally then install Hugo on your machine and build the website by running, in the root folder, the following:

```bash
hugo -D
```

and files will be placed in the doc folder.

## Adding content

The content of the site can be found in the various markdown folders in this repository. For instance, the content of the about page is [here](https://github.com/RSE-Midlands/rse-midlands.github.io/blob/main/content/docs/about.md) and the recent event [here](https://github.com/RSE-Midlands/rse-midlands.github.io/blob/main/content/docs/event-8th-June.md).

The site has a blog format. Posts placed in the content/posts folder will be added as new posts. For an example post, see the previous [event blog post](https://github.com/RSE-Midlands/rse-midlands.github.io/blob/bdac4cc7f914fa4d1e486d0861c2c6ffb8ef3ca8/content/posts/inaugural-meeting.md). The information on the front page was added by changing the theme index layout (which you can see [here](https://github.com/RSE-Midlands/rse-midlands.github.io/blob/main/themes/mainroad/layouts/index.html)).

Any images or other static content should be added to the [static folder](https://github.com/RSE-Midlands/rse-midlands.github.io/tree/main/static).
