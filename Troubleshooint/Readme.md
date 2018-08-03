

# Error Messages

## "Some objects were not cleaned up when closing the scene"

This error message is caused when a game object is added to a scene when it is closing or the app is shutting down.  The usual culprit of this OnDestroy, which is called in those two situations.  The easiest way to prevent this error is to not create game objects in OnDestroy or in a method called by OnDestroy.

