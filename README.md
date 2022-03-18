# RSE Midlands Website

The website can be found at [rse-midlands.github.io](https://rse-midlands.github.io). The website is built using [hugo](https://gohugo.io/).

To build the website, add or alter .md files in the content folder, then run

```bash
hugo -D
```

and files will be placed in the doc folder. The location of these outputs is important as GitHub expects the files to be in the folder root or doc folder.

To view the content using hugo server.

```bash
hugo server
```

## Devcontainer

We build the site within a [devcontainer](https://code.visualstudio.com/docs/remote/containers) using Visual Studio Code. If you open the folder within Visual Studio Code, have docker installed and the remotes-containers extension installed, then you will see a prompt to build and enter the container.

Within the container, you can build the website using the below command.

```bash
hugo -D
```

I found that port forwarding was not working within Visual Studio Code (and so the hugo server command would be no use). I fixed this by going to the doc folder in powershell (within Windows) and starting the Python web server using the below command.

```bash
python -m http.server
```

You should then be able to view the content by going to 127.0.0.1:8000 in your browser.
