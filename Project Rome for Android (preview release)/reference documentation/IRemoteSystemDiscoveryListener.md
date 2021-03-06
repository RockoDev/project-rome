# IRemoteSystemDiscoveryListener interface
Interface to handle remote system discovery events.

## Syntax
`public interface IRemoteSystemDiscoveryListener`

## Public methods

### onRemoteSystemAdded
Called when a remote system is discovered.

`void onRemoteSystemAdded(RemoteSystem remoteSystem)`

**Parameters**  
*remoteSystem* - a **RemoteSystem** object representing the discovered device.

### onRemoteSystemUpdated
Called when a previously discovered remote system has been updated as being available by another protocol. This update should be reflected in the app's reference to this remote system.

`void onRemoteSystemUpdated(RemoteSystem remoteSystem)`

**Parameters**  
*remoteSystem* - the **RemoteSystem** object representing the device that was updated
    
### onRemoteSystemRemoved
Called when a previously discovered remote system is no longer available.

`void onRemoteSystemRemoved(String remoteSystemId)`

**Parameters**  
*remoteSystemId* - the unique device id of the removed remote system
