## 3.4 DevOps - Infrastructure as Code with Terraform
Deploying the Azure Infrastructure and the container workload may seem like two different problems, but they are both infrastructure deployment concerns. Wouldn't it be great to be able to use one tool to recreate the entire environment? Let's start with deploying AKS.

# 3.4.0 Tasks
Use Terraform to deploy AKS, and deploy your helm charts

https://www.terraform.io/intro/index.html
https://docs.microsoft.com/en-us/azure/terraform/terraform-create-k8s-cluster-with-tf-and-aks


## 3.4.1 DevOp - Kubernetes as Code with Terraform
Now that AKS is up and running, we can deploy the Helm chart we created in a prior exercise to the AKS cluster we just created.

# 3.4.1 Tasks
Deploy helm chart to new AKS cluster.

https://www.terraform.io/docs/providers/helm/index.html

`HINT 1: Create a seperate folder for this Terraform code. Terraform treats each folder entirely seperate, and this should simplify dependancies.`

`HINT 2: The Helm provider should be able to use the KUBECONFIG exported in the last step of 3.4.0. Use kubectl to ensure it's configured correctly. Advanced topic - use remote data sources to pull in information from the state file created for 3.4.0.

https://www.terraform.io/docs/providers/terraform/d/remote_state.html`
