# Level 1: Load Balancers

## Getting Started with BigQuery ML
```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Getting%20Started%20with%20BigQuery%20Machine%20Learning/quicklabgsp247.sh
sudo chmod +x quicklabgsp247.sh
./quicklabgsp247.sh
```

## Google Kubernetes Engine: Qwik Start

```cmd
export ZONE=
```

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Google%20Kubernetes%20Engine%20Qwik%20Start/quicklabgsp100.sh
sudo chmod +x quicklabgsp100.sh
./quicklabgsp100.sh
```

## Set Up Network and HTTP Load Balancers
```cmd
export ZONE=
```

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Set%20Up%20Network%20and%20HTTP%20Load%20Balancers/quicklabgsp007.sh
sudo chmod +x quicklabgsp007.sh
./quicklabgsp007.sh
```

## Introduction to Docker

```cmd
export REGION=
```

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Introduction%20to%20Docker/quicklabgsp055.sh
sudo chmod +x quicklabgsp055.sh
./quicklabgsp055.sh
```

## Deploy Your Website on Cloud Run

```cmd
export REGION=
```

```cmd
export REGION=
gcloud services enable artifactregistry.googleapis.com \
cloudbuild.googleapis.com \
run.googleapis.com
git clone https://github.com/googlecodelabs/monolith-to-microservices.git
cd ~/monolith-to-microservices
./setup.sh
cd ~/monolith-to-microservices/monolith
gcloud artifacts repositories create monolith-demo --location=$REGION --repository-format=docker
gcloud auth configure-docker $REGION-docker.pkg.dev
gcloud builds submit --tag $REGION-docker.pkg.dev/$DEVSHELL_PROJECT_ID/monolith-demo/monolith:1.0.0
gcloud run deploy monolith --image $REGION-docker.pkg.dev/$DEVSHELL_PROJECT_ID/monolith-demo/monolith:1.0.0 --allow-unauthenticated --region $REGION
gcloud run deploy monolith --image $REGION-docker.pkg.dev/$DEVSHELL_PROJECT_ID/monolith-demo/monolith:1.0.0 --allow-unauthenticated --region $REGION --concurrency 1
gcloud run deploy monolith --image $REGION-docker.pkg.dev/$DEVSHELL_PROJECT_ID/monolith-demo/monolith:1.0.0 --allow-unauthenticated --region $REGION --concurrency 80
cd ~/monolith-to-microservices/react-app/src/pages/Home
mv index.js.new index.js
cd ~/monolith-to-microservices/react-app
npm run build:monolith
cd ~/monolith-to-microservices/monolith
gcloud builds submit --tag $REGION-docker.pkg.dev/$DEVSHELL_PROJECT_ID/monolith-demo/monolith:2.0.0
gcloud run deploy monolith --image $REGION-docker.pkg.dev/$DEVSHELL_PROJECT_ID/monolith-demo/monolith:2.0.0 --allow-unauthenticated --region $REGION
```

## Create an Internal Load Balancer

```cmd
export REGION=
export ZONE_1=
export ZONE_2=
```

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/July%20updated%20Create%20an%20Internal%20Load%20Balancer/quicklabgsp216.sh
sudo chmod +x quicklabgsp216.sh
./quicklabgsp216.sh
```


## Cloud Natural Language API: Qwik Start

Run in ssh 

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Cloud%20Natural%20Language%20API%20Qwik%20Start/quicklabgsp097.sh
sudo chmod +x quicklabgsp097.sh
./quicklabgsp097.sh
```

## GKE Workload Optimization

https://github.com/CloudHustlers/Level1-March24/blob/main/GKE%20Workload%20Optimization%20%23GSP769%20.md

## Cloud Source Repositories: Qwik Start

```cmd
gcloud source repos create REPO_DEMO
```

## Working with JSON, Arrays, and Structs in BigQuery

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Working%20with%20JSON%20Arrays%20and%20Structs%20in%20BigQuery/quicklabgsp416.sh
sudo chmod +x quicklabgsp416.sh
./quicklabgsp416.sh
```

## Publish your AppSheet App

## Pub/Sub: Qwik Start - Python

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/PubSub%20Qwik%20Start%20Python/quicklabgsp094.sh
sudo chmod +x quicklabgsp094.sh
./quicklabgsp094.sh
```
