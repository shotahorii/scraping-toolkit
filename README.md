# scraping-toolkit
A toolkit for scraping with python / jupyter. 

## Getting Started

### Prerequisites
- docker installed 
- jupyter/scipy-notebook image is pulled by docker pull jupyter/scipy-notebook

### Build a docker image for this repo's environment

`cd` to the directory where Dockerfile is located, then type below. 

```
docker build -t shotahorii/scraping-toolkit-env .
```
Note1: `shotahorii/scraping-toolkit-env` in the command above is the name of the docker image. This can be any other name that you'd like to call this image.   
Note2: Don't forget `.` at the end of the command. 

### Run

```
docker run --rm -p 8888:8888 -v "$PWD":/home/jovyan/work shotahorii/scraping-toolkit-env
```