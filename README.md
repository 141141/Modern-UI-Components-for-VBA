# VBA_TOOLS
Add this Dll to your VBA projects and have some cool features.

# [List of futures]
### [Show non-blocking notifications]
Inspired from Toastr (https://github.com/CodeSeven/toastr).
Allowing VBA users to show simple notifications without having to wait or stress their VBA applications.
Good for showing notifications that do not require user action.

![just a notification](https://raw.githubusercontent.com/krishKM/VBA_TOOLS/master/information.png)

Customise your notification like you want:

![picture of 3 notifications](https://raw.githubusercontent.com/krishKM/VBA_TOOLS/master/collections.png)
```VBA
'used commands
fn_toast_dll "Ups something went wrong!",vberror,0
fn_toast_dll "Yellow weather warning!",vbexclamation,0
fn_toast_dll "You've just received a notification",vbinformation,0
```

in Action
![Notification in action gif](https://github.com/krishKM/VBA_TOOLS/blob/master/InAction.gif)

### [Receive SignalR Messages]
This works for me because I do have own signalR server but generally is under development or say not ready yet!
It's like google push messages or any other push message service. You can send notification to all of your logged in yours from one place.
Expanding this, you could also use as a chat server where all logged in participants could send and receive messages among them.
Again without stressing VBA apps.


### ByteToImage
ByteToImage(byte[] byteArraym string TemporaryPath, bool useCache) is a function for MS Access users. Basically you can convert a byteARray received from database into a pictures.
Will return the path of the image file. Use the path as image location for your image property.
something like Me.Image32.Picture = gDll.ByteToImage(ByteArray, "SaveLocationPath")
