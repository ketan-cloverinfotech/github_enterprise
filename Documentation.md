# Create azure github server with following command
**Step 1: Create azure vm**
```
az vm create \
  --resource-group azure-server \
  --name ghes-server-1 \
  --image GitHub:GitHub-Enterprise:GitHub-Enterprise:latest \
  --size Standard_D4s_v3 \
  --os-disk-name ghes-os-disk \
  --admin-username azureuser \
  --admin-password MyS3cureP@ssword! \
  --location eastus
```
**Note: You have change vm type and attach disk size of 150GB with specail SSD**


you will get following error even when you attach secondary disk,

![Screenshot 2025-06-26 164308](https://github.com/user-attachments/assets/e910ab03-7638-40cc-8629-1509f3b13575)


**You have to wait 5 mins because we attached disk it does not refrected so wait for 5mins**


