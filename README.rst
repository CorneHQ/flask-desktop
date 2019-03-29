flask-desktop
=====

flask-desktop is a Python module that allows you to convert Flask apps into cross platform desktop apps with three lines of code.

Installation:
-------------
::

    pip install git+git://github.com/CorneHQ/flask-desktop.git

I'd like to have flask-desktop available on pip, but currently don't have the time and headspace to make that happen. If you want this to happen, please do it and I'll add you as a collaborator to this repo.

Usage:
------
::

    from webui import init_gui 
    from flask import Flask, render_template, request
    
    app = Flask(__name__)

    # FLASK HERE

    if __name__ == '__main__':
      init_gui(app)


flask-desktop is powered by PyQt5, and should run on Windows, Mac and Linux. You can even create standalone executables using PyInstaller!

Parameters:
-------
::
init_gui(application, port=5000, width=300, height=400, window_title="PyFladesk", icon="appicon.png", argv=None)

License
-------
flask-desktop is licensed under the MIT License. See the LICENSE file for more details.
