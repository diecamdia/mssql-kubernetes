# MSSQL on AZURE-Kubernetes

Repository to implement a MSSQL Express Instance on Azure Kubernetes Services.

Must create a secret before apply de File.

> `kubectl create secret generic mssql --from-literal=SA_PASSWORD="Y0urC0m9l&xP@ssw0rd"`

Create Storage Class Name and Persistent Volume Claim

> `kubectl apply -f pvc.yaml`

Create Deployment

> `kubectl apply -f sqldeployment.yaml`

This information is from [Microsoft documentation](https://docs.microsoft.com/es-es/sql/linux/tutorial-sql-server-containers-kubernetes?view=sql-server-ver15)



