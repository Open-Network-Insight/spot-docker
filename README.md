# **Apache Spot (Incubating)**   

Apache Spot is open source software for leveraging insights from flow and packet analysis. It helps enterprises and service providers gain insight on their compute environments through transparency of service delivery and identification of potential security threats or attacks happening among resources operating at cloud scale.

While current threat intelligence tools help, identifying unknown threats and attacks remains a challenge. Apache Spot provides tools to accelerate companies’ ability to expose suspicious connections and previously unseen attacks using flow and packet analysis technologies. 
<br><br>

## **Project Structure**

Each project sub folder is intended to be the source for the [Apache Spot organization](https://hub.docker.com/u/apachespot/) on the [Docker Hub](https://docs.docker.com/docker-hub/)

### *spot-dev*

The spot-dev image is a full development virtual machine that contains the following:

* Development Dependencies
* Working CDH distribution
* links to synthetic data

### *spot-demo*

the spot-demo is the source for apachespot/spot-demo

## **Prerequisites**

* Docker

## **Build**

for an example build we will use the `spot-demo`

1. download source code `git clone https://github.com/Open-Network-Insight/spot-docker`

2. select project folder `cd spot-demo`

3. build image `docker build -t spot-demo .`

    a. the `-t [value] names and optionally tags the build image`

    b. the `.` tells docker to look in the current folder for the `Dockerfile`

4. run the image `docker run -it -p 8889:8889 spot-demo`

## **Needs**

* Automation scripts to download code from git repository at build time
* Automated builds
