

# Error Messages
Special thanks to [this post](https://answers.unity.com/questions/155200/stuff-is-going-wacky-checklist-compiler-errors-syn.html) for many of the error messages.  

## !slot->GetLocalAABB().IsValid()
This can be caused by an object having a scale of zero or a very large number.
http://answers.unity3d.com/questions/8276/what-causes-error-sh-maabbisvalid.html
http://answers.unity3d.com/questions/11016/what-does-slot-getlocalaabbisvalid-mean.html

## "Some objects were not cleaned up when closing the scene"

This error message is caused when a game object is added to a scene when it is closing or the app is shutting down.  The usual culprit of this OnDestroy, which is called in those two situations.  The easiest way to prevent this error is to not create game objects in OnDestroy or in a method called by OnDestroy.

Posts on the error message.

* [https://answers.unity.com/questions/1274772/some-objects-were-not-cleaned-up-when-closing-the-4.html](https://answers.unity.com/questions/1274772/some-objects-were-not-cleaned-up-when-closing-the-4.html)

[https://feedback.unity3d.com/suggestions/improve-some-objects-were-not-cleaned-up-when-closing-the-scene-error-message](https://feedback.unity3d.com/suggestions/improve-some-objects-were-not-cleaned-up-when-closing-the-scene-error-message)

