# Personal academic website
**Built using the Academic Pages template**

## Table of contents
- [How to run locally](#how-to-run-locally)
- [Run using Docker](#run-using-docker)

---

### How to run locally

Make sure you have ruby-dev, bundler, nodejs and some additional dependencies installed.
```bash
sudo apt install ruby-dev ruby-bundler nodejs build-essential gcc make
```
Run `bundle install` to install ruby dependencies.

Run `jekyll serve -l -H localhost` to generate the HTML and serve it from `localhost:4000` the local server will automatically rebuild and refresh the pages on change to Markdown (*.md) and HTML files, while changes to the core template and configuration (i.e., `_config.yml`) will require stoping and restarting Jekyll.

If you are running on Linux it may be necessary to install some additional dependencies prior to being able to run locally: ``

### Run using Docker

Working from a different OS, or just want to avoid installing dependencies? You can use the provided `Dockerfile` to build a container that will run the site for you if you have [Docker](https://www.docker.com/) installed.

You can build and execute the container by running the following command in the repository:

```bash
chmod -R 777 .
docker compose up
```

You should now be able to access the website from `localhost:4000`.
