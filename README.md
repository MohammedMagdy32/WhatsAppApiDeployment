
# WhatsAppApi Deployment 
This document shows you how to set up a Multiple instances of the WhatsApp Business API client on a single machine machine.

## Pre-requisites
- Install Docker from the following [link](https://docs.docker.com/compose/install/?fbclid=IwAR3Qui2fC8-Q3O4qgOEbCERv0l-HSViw80k3pN3xWvLZcakyeasvMMnctzE)

## Deployment
1. Clone this repo into your machine

2. Open the folder correponding to related app/port for example will open first instance 9090
```sh
cd WhatsAppApiDeplyment/infrastucutre/app1-9090
```

3. Run the following command to bring the app up 
```sh
export WA_API_VERSION=3.35.4; docker-compose up -d
```
 
4. Repeat 2,3 for each app instance by switching between folders under infrastucutre folder based on port 9091,9092,9093,9094,9095

### Note

To create new instance of the App, follow the below instruction

- ewewew
- ewewe
- ewewe

## Validation
To make sure the app up and running, run the below command
```sh
curl --location --request POST 'https://machineHostIp:PortNumber/v1/users/login' \
--header 'Content-Type: application/json' \
--header 'Authorization: Basic YWRtaW46c2VjcmV0' \
--data-raw '{
    "new_password": "your password"
}'
```

