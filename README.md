# CodeWisdom-aiAssistant
CodeWisdom-aiAssistant release
CodeWisdom-aiAssistant is a plugin of IntelliJ IDEA based on big data and deep learning, which provides following features:
* Recommend top-10 APIs for one line at a time. The APIs include API method calls, API field accesses in JDK 1.8 library and control structures such as if, while.
* Complete arguments (parameters) in each recommended API.
* Auto-add import information when a recommended API is selected.
* Provide API description of each recommended API.

# Installation tutorial
For Windows: File -> Settings -> Plugins -> Install plugin from disk... -> find and choose the 'CodeWisdom-aiAssistant.jar'
For Mac: IntelliJ IDEA -> Preferences -> Plugins -> Install plugin from disk... -> find and choose the 'CodeWisdom-aiAssistant.jar'.
# How-to-use
Put the cursor to the line that needs API recommendations and then press the shortcut key "ctrl+alt+0" or put the cursor to the line that needs API recommendations, press the right mouse button to get a pop menu and then press "CodeWisdom-aiAssistant" in the pop menu.
# Notes
## 1.Note that CodeWisdom-aiAssistant just supports to recommend APIs in JDK(Java Development Kit)1.8, other librarys are not supported now.
## 2.Note that the following usages of CodeWisdom-aiAssistant are allowed:
### 2.1 Recommend a whole line API call:
![image](https://github.com/FudanSELab/CodeWisdom-aiAssistant/blob/master/Notes/one_line_code_note.jpg)
### 2.2 Recommend the API condition in control structures such as 'if', 'while' and 'for':
![image](https://github.com/FudanSELab/CodeWisdom-aiAssistant/blob/master/Notes/note3.jpg)
![image](https://github.com/FudanSELab/CodeWisdom-aiAssistant/blob/master/Notes/note5.jpg)
![image](https://github.com/FudanSELab/CodeWisdom-aiAssistant/blob/master/Notes/note10.jpg)
## 3.Note that the following usages of CodeWisdom-aiAssistant are not allowed:
### 3.1 Recommend the API call when given its receiver (e.g. file.$hole$):
![image](https://github.com/FudanSELab/CodeWisdom-aiAssistant/blob/master/Notes/note4.jpg)
### 3.2 Recommend the API condition in for($hole$):
![image](https://github.com/FudanSELab/CodeWisdom-aiAssistant/blob/master/Notes/note9.jpg)
### 3.3 Recommend the API call when it is the parameter of another API call. In this situation CodeWisdom-aiAssistant can give recommendations, but the recommendations may be not accurate:
![image](https://github.com/FudanSELab/CodeWisdom-aiAssistant/blob/master/Notes/note8.jpg)
