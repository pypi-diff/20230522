# Comparing `tmp/flapgui-0.4.0.tar.gz` & `tmp/flapgui-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flapgui-0.4.0.tar", last modified: Mon May 15 17:41:21 2023, max compression
+gzip compressed data, was "flapgui-0.5.0.tar", last modified: Mon May 22 17:37:15 2023, max compression
```

## Comparing `flapgui-0.4.0.tar` & `flapgui-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-15 17:41:21.221648 flapgui-0.4.0/
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     1073 2023-05-12 20:35:47.000000 flapgui-0.4.0/LICENSE
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     1221 2023-05-15 17:41:21.221023 flapgui-0.4.0/PKG-INFO
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      680 2023-05-15 17:41:00.000000 flapgui-0.4.0/README.md
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      614 2023-05-15 15:53:57.000000 flapgui-0.4.0/pyproject.toml
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)       38 2023-05-15 17:41:21.221852 flapgui-0.4.0/setup.cfg
-drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-15 17:41:21.147452 flapgui-0.4.0/src/
-drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-15 17:41:21.150807 flapgui-0.4.0/src/flapgui/
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)    14404 2023-05-15 17:32:37.000000 flapgui-0.4.0/src/flapgui/__init__.py
-drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-15 17:41:21.217641 flapgui-0.4.0/src/flapgui.egg-info/
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     1221 2023-05-15 17:41:21.000000 flapgui-0.4.0/src/flapgui.egg-info/PKG-INFO
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      196 2023-05-15 17:41:21.000000 flapgui-0.4.0/src/flapgui.egg-info/SOURCES.txt
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        1 2023-05-15 17:41:21.000000 flapgui-0.4.0/src/flapgui.egg-info/dependency_links.txt
--rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        8 2023-05-15 17:41:21.000000 flapgui-0.4.0/src/flapgui.egg-info/top_level.txt
+drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-22 17:37:15.638618 flapgui-0.5.0/
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     1073 2023-05-12 20:35:47.000000 flapgui-0.5.0/LICENSE
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     4179 2023-05-22 17:37:15.637987 flapgui-0.5.0/PKG-INFO
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     3639 2023-05-20 19:49:28.000000 flapgui-0.5.0/README.md
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      614 2023-05-22 17:36:25.000000 flapgui-0.5.0/pyproject.toml
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)       38 2023-05-22 17:37:15.638789 flapgui-0.5.0/setup.cfg
+drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-22 17:37:15.576226 flapgui-0.5.0/src/
+drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-22 17:37:15.606172 flapgui-0.5.0/src/flapgui/
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)    12878 2023-05-22 17:34:48.000000 flapgui-0.5.0/src/flapgui/__init__.py
+drwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        0 2023-05-22 17:37:15.635329 flapgui-0.5.0/src/flapgui.egg-info/
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)     4179 2023-05-22 17:37:15.000000 flapgui-0.5.0/src/flapgui.egg-info/PKG-INFO
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)      196 2023-05-22 17:37:15.000000 flapgui-0.5.0/src/flapgui.egg-info/SOURCES.txt
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        1 2023-05-22 17:37:15.000000 flapgui-0.5.0/src/flapgui.egg-info/dependency_links.txt
+-rwxrwxrwx   0 winfan3672  (1000) winfan3672  (1000)        8 2023-05-22 17:37:15.000000 flapgui-0.5.0/src/flapgui.egg-info/top_level.txt
```

### Comparing `flapgui-0.4.0/LICENSE` & `flapgui-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flapgui-0.4.0/pyproject.toml` & `flapgui-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "flapgui"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="WinFan3672", email="winfan3672@gmail.com" },
 ]
 description = "Easy-to-use and cross-platform GUI library for making functional GUI apps"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `flapgui-0.4.0/src/flapgui/__init__.py` & `flapgui-0.5.0/src/flapgui/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,33 @@
+#!/usr/bin/python
+
+# FlapGUI 0.5
+
 import tkinter as tk
 from tkinter import filedialog
 from tkinter import messagebox
 from tkinter import ttk
 import tkinter.colorchooser
 import webbrowser
+import functools
 
 global app_version
-app_version = [0,4,0]
+app_version = [0,5,0]
 global verbose
 verbose = False
 
+def ignore_tcl_error(func):
+    @functools.wraps(func)
+    def wrapper(*args, **kwargs):
+        try:
+            return func(*args, **kwargs)
+        except tk.TclError:
+            pass  # Ignore the error
+    return wrapper
+
 def window(title="flapWindow", width=250, height=250):
     """
 Creates a window.
     """
     if verbose:
         print(f"Flap: Created window \"{title}\" with resolution {width}x{height}")
     window = tk.Tk()
@@ -40,158 +54,110 @@
     Args:
         element (tkinter.Widget): The tkinter widget to be disabled.
     """
     if isinstance(element, tk.Menu):
         element.entryconfig(0, foreground='gray')
     else:
         element.configure(state='disabled')
-##class CheckBox:
-##    def __init__(self, root, label, defaultState=False, boxColor=None, checkColor=None):
-##        self.var = tk.BooleanVar(value=defaultState)
-##        
-##        if ttk.Style().theme_use() == 'default':
-##            self.checkbox = ttk.Checkbutton(root, text=label, variable=self.var)
-##            changeWidgetColor(self.checkbox, boxColor, checkColor)
-##        else:
-##            style = ttk.Style()
-##            style.configure('Custom.TCheckbutton', background=boxColor, indicatorcolor=checkColor)
-##            self.checkbox = ttk.Checkbutton(root, text=label, variable=self.var, style='Custom.TCheckbutton')
-##        
-##        self.checkbox.pack()
-##
-##    def get_state(self):
-##        return self.var.get()
-##
-##class StyledCheckbox(tk.Frame):
-##    def __init__(self, master=None, cnf={}, **kw):
-##        super().__init__(master, cnf, **kw)
-##        self.toggle_var = tk.BooleanVar(value=False)
-##
-##        self.checkbox_frame = tk.Frame(self)
-##        self.checkbox_frame.pack(side='left')
-##
-##        self.checkbox_label = tk.Label(
-##            self.checkbox_frame,
-##            text='\u2713',  # Unicode character for checkmark
-##            font=('Arial', 12),
-##            bg=self['bg']
-##        )
-##        self.checkbox_label.pack()
-##
-##        self.checkbox_text = tk.Label(
-##            self,
-##            text=self['text'],
-##            font=self['font'],
-##            bg=self['bg']
-##        )
-##        self.checkbox_text.pack(side='left')
-##
-##        self.bind('<Button-1>', self.toggle)
-##
-##    def toggle(self, event):
-##        self.toggle_var.set(not self.toggle_var.get())
-##        if self.toggle_var.get():
-##            self.checkbox_label.config(fg='green')
-##        else:
-##            self.checkbox_label.config(fg='black')
-##
-##    def get_state(self):
-##        return self.toggle_var.get()
-##
-##
-##    def get_state(self):
-##        return self.toggle_var.get()
-##class CustomCheckBox(ttk.Checkbutton):
-##    def __init__(self, master=None, accent_color=None, *args, **kwargs):
-##        self.accent_color = accent_color
-##        super().__init__(master, *args, **kwargs)
-##        self.style = ttk.Style()
-##        self.style.theme_use('clam')  # Use 'clam' theme for consistent look across platforms
-##
-##        # Configure the style for the checkbox
-##        self.style.configure('CustomCheckBox.TCheckbutton',
-##                             indicatorsize=20,
-##                             background='white',
-##                             relief='flat',
-##                             borderwidth=0)
-##        self.style.map('CustomCheckBox.TCheckbutton',
-##                       foreground=[('active', self.accent_color)],
-##                       background=[('active', 'white')])
-##
-##        # Create the checkbox with the custom style
-##        self.configure(style='CustomCheckBox.TCheckbutton')
-##
-##    def set_accent_color(self, accent_color):
-##        self.accent_color = accent_color
-##        self.style.map('CustomCheckBox.TCheckbutton',
-##                       foreground=[('active', self.accent_color)])
-##
-##
-class Checkbox:
-    def __init__(self, root, label, isChecked=False, boxColor=None, textColor=None, fillColor=None, bgColor=None):
-        self.root = root
-        self.label = label
-        self.isChecked = isChecked
-        self.boxColor = boxColor
-        self.textColor = textColor
-        self.fillColor = fillColor
-        self.bgColor = bgColor
-        
-        self.checkbox_var = tk.BooleanVar(value=self.isChecked)
-        self.checkbox = tk.Checkbutton(
-            self.root,
-            text=self.label,
-            variable=self.checkbox_var,
-            onvalue=True,
-            offvalue=False,
-            command=self._on_checkbox_changed
-        )
-        self.checkbox.pack()
-        
-        if self.boxColor:
-            self.checkbox.config(activeforeground=self.boxColor, fg=self.boxColor)
-            self.checkbox.config(selectcolor=self.boxColor)
-        if self.textColor:
-            self.checkbox.config(activeforeground=self.textColor)
-        if self.fillColor:
-            self.checkbox.config(activebackground=self.fillColor)
-        if self.bgColor:
-            self.checkbox.config(background=self.bgColor)
-        
-    def _on_checkbox_changed(self):
-        self.isChecked = self.checkbox_var.get()
-        
-    def getCheckboxState(self):
-        return self.isChecked
+def changeAlignment(widget, alignment):
+    """
+    Aligns a widget to a specific alignment.
+
+    Args:
+        widget: The widget to be aligned.
+        alignment: The desired alignment. Possible values: 'left', 'right', 'top', 'bottom', 'center'.
 
+    Raises:
+        ValueError: If an invalid alignment value is provided.
+    """
+    valid_alignments = ['left', 'right', 'top', 'bottom', 'center']
+
+    if alignment not in valid_alignments:
+        raise ValueError("Invalid alignment value. Please use one of the following: 'left', 'right', 'top', 'bottom', 'center'.")
+
+    # Clear any existing alignment
+    widget.pack_forget()
+    widget.pack(fill=tk.BOTH, expand=True)
+
+    if alignment == 'left':
+        widget.pack_configure(anchor=tk.W)
+    elif alignment == 'right':
+        widget.pack_configure(anchor=tk.E)
+    elif alignment == 'top':
+        widget.pack_configure(anchor=tk.N)
+    elif alignment == 'bottom':
+        widget.pack_configure(anchor=tk.S)
+    elif alignment == 'center':
+        widget.pack_configure(anchor=tk.CENTER)
+def createCheckbox(root, label, isChecked=False, fg="black"):
+    checkbox_var = tk.BooleanVar(value=isChecked)
+    checkbox = tk.Checkbutton(root, text=label, variable=checkbox_var, fg=fg)
+    checkbox.pack()
+    return checkbox
+
+def getCheckboxState(checkbox):
+    checkbox_var = checkbox.cget("variable")
+    return checkbox_var.get()
+@ignore_tcl_error
 def changeWidgetColor(widget, background_color, text_color=None):
-    widget.config(selectcolor=background_color)
+    widget.configure(selectcolor=background_color)
     if text_color:
-        widget.config(fg=text_color)
+        widget.configure(fg=text_color)
     widget.update_idletasks()
-
+@ignore_tcl_error
 def changeAccentColor(root, background_color, text_color=None):
     root.tk_setPalette(background=background_color)
     for widget in root.winfo_children():
         if isinstance(widget, tk.Checkbutton):
             changeWidgetColor(widget, background_color, text_color)
         else:
             changeWidgetColor(widget, background_color, text_color)
             if isinstance(widget, tk.Toplevel):
                 changeAccentColor(widget, background_color, text_color)
-def resetAccentColor(root):
-    r = window()
-    x = root.cget("background")
-    print("DefaultBGColor:",x)
-    r.destroy()
-    changeAccentColor(root,x)
+def createDropDown(root, strings=[]):
+    # Create a drop down widget
+    drop_down = ttk.Combobox(root, values=strings)
+    drop_down.pack()
+    
+    return drop_down
+
+def getDropDownState(drop_down):
+    # Get the selected option in the drop down
+    selected_option = drop_down.get()
+    
+    return selected_option
+
+def createRadioButtons(root, buttons=[],alignment=None):
+    # Create radio buttons
+    selected_button = tk.StringVar()
+    
+    for button_text in buttons:
+        radio_button = tk.Radiobutton(root, text=button_text, variable=selected_button, value=button_text)
+        if alignment:
+            changeAlignment(radio_button,alignment)
+        radio_button.pack(anchor=tk.W)
+    
+    return selected_button
+
+def getRadioButtonState(radio_buttons):
+    # Get the selected radio button's value
+    selected_value = radio_buttons.get()
+    
+    return selected_value
 def createFrame(root):
     frame = tk.Frame(root)
     frame.pack()
     return frame
+def lockWindowPos(root):
+    """Locks the window from being moved at its current position."""
+    root.attributes("-topmost", True)
+
+def unlockWindowPos(root):
+    """Allows the window to be moved."""
+    root.attributes("-topmost", False)
 def createHyperlinkText(root, label_text, url):
     label = tk.Label(root, text=label_text, fg='blue', cursor='hand2')
     label.pack()
     label.bind('<Button-1>', lambda e: webbrowser.open(url))
 def changeTitle(root, new_title):
     root.title(new_title)
 def autoScaleResolution(window):
@@ -298,21 +264,25 @@
 
     def configure_scrollbar(event):
         canvas.configure(scrollregion=canvas.bbox("all"), width=200, height=200)
 
     content_frame.bind("<Configure>", configure_scrollbar)
 
     return content_frame
-def messageBox(title,message):
-    msg=message.replace("\n","\\n")
-    print(f"Flap: Message Box: {title} :: \"{msg}\"")
-    root = tk.Tk()
-    root.withdraw() # hide the main window
-
-    messagebox.showinfo(title, message)
+def messageBox(title,message,root=None):
+    if root:
+        w=subWindow(root,title)
+    else:
+        w=window(title)
+    addText(w,message)
+    createButton(w,"OK",w.destroy)
+    keyBind(w,"<Return>",lambda event:w.destroy())
+    keyBind(w,"<Escape>",lambda event:w.destroy())
+    keyBind(w,"<Control-q>",lambda event:w.destroy())
+    autoScaleResolution(w)
 def addScrollbar(root, text):
     scrollbar = tk.Scrollbar(root)
     scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
     scrollbar.config(command=text.yview)
     text.config(yscrollcommand=scrollbar.set)
     text.pack(side=tk.LEFT, fill=tk.BOTH, expand=True)
     scrollbar.pack(side=tk.RIGHT, fill=tk.Y)
@@ -383,15 +353,18 @@
     if color:
         r, g, b = map(int, color[0])
         return f"#{r:02x}{g:02x}{b:02x}"
     else:
         return None
 def getVersion():
     return app_version
-
+def lockWindowSize(root):
+    root.resizable(0, 0)
+def unlockWindowSize(root):
+    root.resizable(1, 1)
 class FlowLayout(tk.Frame):
     def __init__(self, master, **kwargs):
         super().__init__(master, **kwargs)
         self.widgets = []
 
     def add_widget(self, widget):
         self.widgets.append(widget)
@@ -414,10 +387,8 @@
     button.pack()
     flowLayout.add_widget(button)
 
 def addFlowText(flowLayout, label):
     text = tk.Label(flowLayout, text=label)
     text.pack()
     flowLayout.add_widget(text)
-
-if verbose:
-    print(f"Flap: Initialised Framework ({app_version[0]}.{app_version[1]}.{app_version[2]})")
+print(f"Flap: Initialised Framework ({app_version[0]}.{app_version[1]}.{app_version[2]})")
```

