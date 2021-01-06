PyGUIBox  |  Version 0.3
=========

PyGUIBox is a simple cross-platform tool for creating GUI message boxes.

```pip install pyguibox```

Example Usage
=============

Show an custom message box
--------------------------

Displays the box message that you have customized.<br>
You can customize the icons and buttons in this section.<br>
Acceptable icons = 1, 2, 3<br>
Acceptable modes = 1, 2, 3, 4, 5<br>
-----[ Icons ]-----<br>
1 : Warning icon<br>
2 : Info icon<br>
3 : Error icon<br>
-----[ Modes Buttons ]-----<br>
1 : Ok<br>
2 : Ok, Cancel<br>
3 : Yes, No, Cancel<br>
4 : Yes, No<br>
5 : Ok, Help<br>

Returns the text of the button clicked on.<br>
* You can also set the title of the message box.<br>
Buttons for this message: OK<br>

```python
    >>> import pyguibox
    >>> pyguibox.messagebox(message="This is a test", title="Test Title", mode=3, icon=3)
    'Yes'
    >>> pyguibox.messagebox(message="This is a test", title="Test Title", mode=2, icon=2)
    'Cancel'
    >>> pyguibox.messagebox(message="This is a test", title="Test Title", mode=1, icon=1)
    'OK'
```

Show an alert box
--------------------------

Displays a simple message box with text and a single OK button.<br>
Returns the text of the button clicked on.<br>
* You can also set the title of the message box.<br>
Buttons for this message: OK<br>

```python
    >>> import pyguibox
    >>> pyguibox.alert("This is a test")
    'OK'
    >>> pyguibox.alert("This is a test", title="Message box title")
    'OK'
```

Show an error box
--------------------------

Displays a simple message box with error icon and a single OK button.<br>
Returns the text of the button clicked on.<br>
* You can also set the title of the message box.<br>
Buttons for this message: OK<br>

```python
    >>> import pyguibox
    >>> pyguibox.error("This is a test")
    'OK'
    >>> pyguibox.error("This is a test", title="Message box title")
    'OK'
```

Show an info box
--------------------------

Displays a simple message box with info icon and a single OK button.<br>
Returns the text of the button clicked on.<br>
* You can also set the title of the message box.<br>
Buttons for this message: OK<br>

```python
    >>> import pyguibox
    >>> pyguibox.info("This is a test")
    'OK'
    >>> pyguibox.info("This is a test", title="Message box title")
    'OK'
```

Show an warn box
--------------------------

Displays a simple message box with warn icon and a single OK button.<br>
Returns the text of the button clicked on.<br>
* You can also set the title of the message box.<br>
Buttons for this message: OK<br>

```python
    >>> import pyguibox
    >>> pyguibox.warn("This is a test")
    'OK'
    >>> pyguibox.warn("This is a test", title="Message box title")
    'OK'
```

Show an confirm box
--------------------------

Displays a simple confirm box.<br>
You can customize the text and title of this message box.<br>
This message box also has the ability to change the mode.<br>
Mode 1 buttons: OK, Cancel<br>
Mode 2 buttons: Yes, No, Cancel<br>
Returns the text of the button clicked on.<br>
* You can also set the title of the message box.<br>
Buttons for this message: OK<br>

```python
    >>> import pyguibox
    >>> pyguibox.confirm("This is a test", mode=1)
    'OK'
    >>> pyguibox.confirm("This is a test", mode=2)
    'Yes'
    >>> pyguibox.confirm("This is a test", mode=1, title="Message box title")
    'Cancel'
    >>> pyguibox.confirm("This is a test", mode=2, title="Message box title")
    'No'
```

Show an input box
--------------------------

Displays a message box with text input.<br>
You can customize the text and title of this message box.<br>
Returns text entered by the user.<br>
(None return: The user has not entered anything)<br>
('Cancel' return: The user has clicked the cancel button)<br>
* You can also set the title of the message box.<br>
Mode 1 buttons: OK, Cancel<br>


```python
    >>> import pyguibox
    >>> pyguibox.prompt("Enter your name :")
    'Cancel'
    >>> pyguibox.prompt("This is a test")
    None
    >>> pyguibox.prompt("This is a test")
    'The Text You Have Entered'
```

Show an password input box
--------------------------

Displays a message box with text input.<br>
(The text entered by the user is displayed as *)<br>
You can customize the text and title of this message box.<br>
Returns text entered by the user.<br>
(None return: The user has not entered anything)<br>
('Cancel' return: The user has clicked the cancel button)<br>
* You can also set the title of the message box.<br>
Mode 1 buttons: OK, Cancel<br>

```python
    >>> import pyguibox
    >>> pyguibox.password("Enter your name :")
    'Cancel'
    >>> pyguibox.password("This is a test")
    None
    >>> pyguibox.password("This is a test")
    'ThePasswordYouHaveEntered'
```

How Does PyGUIBox Work?
========================

This library is currently running on Windows.<br>
After installing the library on the system, you can use the library
