# Logging Client for Unity

Logging Client for Unity. It is useful when your application is unable to run in Unity Editor such as Wikitude or ARCore.

## Usage

* Run [Logging Server](https://github.com/ARX-SKE12/ARTag-Logging-Server)
* Put `LoggingClient/Prefabs/Logging Client.prefab` into your scene.
* Configuration `Url` of Logging Server in Logging Client
* Do Log by `LogClient.instance.Log(TAG_NAME, MESSEGE);`

## Example

```cs
using LoggingClient;
using UnityEngine;

public class ExampleScript : MonoBehaviour {

	// Update is called once per frame
	void Update () {
          LogClient.instance.Log(LogClient.CLIENT_STATUS_TAG, "Test");		
	}
}
```
