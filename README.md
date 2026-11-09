# Unity Touch Input Snippet

A small Unity C# example that distinguishes single-finger taps from directional swipes using the legacy Input API.

## Use it in a Unity scene

1. Copy [PlayerInput](PlayerInput) into your Unity project as `Assets/PlayerInput.cs` so the filename matches the MonoBehaviour.
2. Attach **Player Input** to an active GameObject and make sure the legacy Input Manager is enabled.
3. Test on a touch device and inspect the Unity console.

When a touch ends, movement beyond **15% of the screen height** is classified by its dominant axis. Shorter gestures are logged as taps. The snippet reports the result through `Debug.Log` and can be adapted to call your own gameplay methods.
