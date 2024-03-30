## Arcade Hero: Enter the BigQuery
```cmd
bq --location=US mk --dataset $DEVSHELL_PROJECT_ID:sports
```

## Arcade Hero: Enter the Subnet
```cmd
export REGION=
```

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Arcade%20Hero/quicklabarc127.sh

sudo chmod +x quicklabarc127.sh

./quicklabarc127.sh
```
## Arcade Hero: Enter the BigQuery Table

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Arcade%20Hero/quicklabarc130.sh

sudo chmod +x quicklabarc130.sh

./quicklabarc130.sh
```

## Arcade Hero: Enter the PubSub Subscription

```cmd
curl -LO raw.githubusercontent.com/quiccklabs/Labs_solutions/master/Arcade%20Hero/quicklabarc124.sh

sudo chmod +x quicklabarc124.sh

./quicklabarc124.sh
```

## Arcade Hero: Enter the Inbound Firewall
```cmd
gcloud compute --project=$DEVSHELL_PROJECT_ID firewall-rules create default-allow-inbound --direction=INGRESS --priority=1000 --network=default --action=ALLOW --rules=tcp:80 --source-ranges=0.0.0.0/0 --target-tags=staging-vm
```

## Arcade Hero: Enter the Outbound Firewall
```cmd
gcloud compute --project=$DEVSHELL_PROJECT_ID firewall-rules create default-allow-outbound --direction=EGRESS --priority=1000 --network=default --action=ALLOW --rules=tcp:80 --source-ranges=0.0.0.0/0 --target-tags=staging-vm
```

## Arcade Hero: Enter the Firewall Target Tag

```cmd
gcloud compute --project=$DEVSHELL_PROJECT_ID firewall-rules create default-allow-inbound --direction=INGRESS --priority=1000 --network=default --action=ALLOW --rules=tcp:80 --source-ranges=0.0.0.0/0 --target-tags=staging-vm
```

## Arcade Hero: Enter the Source Repository
```cmd
gcloud source repos create REPO_NAME

gcloud source repos create devsite

```
