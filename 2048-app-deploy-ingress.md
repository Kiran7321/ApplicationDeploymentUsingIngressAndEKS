# 2048 App

## Create Fargate profile

```
eksctl create fargateprofile \
    --cluster demo-cluster \
    --region us-east-1 \
    --name alb-sample-app \
    --namespace game-2048
```

## Deploy the deployment, service and Ingress

```
kubectl apply -f https://raw.githubusercontent.com/kubernetes-sigs/aws-load-balancer-controller/v2.5.4/docs/examples/2048/2048_full.yaml
```


![Screenshot 2024-03-20 at 3 24 56 PM](https://github.com/Kiran7321/ApplicationDeploymentUsingIngressAndEKS/assets/89258260/1af9d5a9-6bd2-434a-a655-54c757d109be)
