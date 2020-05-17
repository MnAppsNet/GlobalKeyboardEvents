# Global Keyboard Events
This is a class that is able to handle multiple events that can be triggered with any keyboard key combination

# How to use
#### -> Create an instance of the class in your main project
#### -> Use method **AddEvent** to assign an event to a specific keystroke
_**public void AddEvent(string name, Keys[] keyStroke, object instance, string method, object[] parameters) :**_
* name : Any name for your event (not used anywhere as for now, the code can be enhanced to use it in the future)
* keyStroke : an array of Keys that you want to trigger your event. The order you put the keys in the array matters.
* instance : an instance from which a method will be called when the event triggered
* method : the method of the instance that will be invoked when the event triggered
* parametes : the parameters to pass to the method, pass null if not any
#### -> You may use the methode AddEvent multiple times to add more than one events
#### -> Use method CaptureKeyboard to start capturing the keyboard keys
#### -> Use method StopCapturingKeyboard to stop it
