# Eventhub-start

# Use
In EventHubSender folder
```
dotnet user-secrets eventhub_connectionstring "<EVENTHUB_CONNECTIONSTRING>"
```
In `Program.cs` of EventHubSender update :
```
        private const string eventHubName = "lpr-poc";
```

In EventHubReceiver folder
```
dotnet user-secrets eventhub_connectionstring "<EVENTHUB_CONNECTIONSTRING>"
dotnet user-secrets blobcontainer_connectionstring "<BLOBCONTAINER_CONNECTIONSTRING>"
```
In `Program.cs` of EventHubReceiver update :
```
        private const string eventHubName = "lpr-poc";
        private const string blobContainerName = "eventhub-test";
```