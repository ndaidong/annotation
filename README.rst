annotation
-----------
Create workspace to annotate image set


Setup tools
~~~~~~~~~~~~~~~~~~~~~~~~~~


Clone this repo, create virtual environment and install recommended packages:

.. code::

  git clone https://github.com/ndaidong/annotation.git
  cd annotation
  python3 -m venv annotation-env
  source annotation-env/bin/activate
  (annotation-env) pip install -r requirements.txt
  (annotation-env) labelImg


Now `labelImg` would be opened with no image nor label loaded:

.. image:: https://i.imgur.com/rhhIVE4.png
     :alt: labelImg - At the first starting

You have to specify the directory where your images are being stored:

.. image:: https://i.imgur.com/I05nCvQ.png
     :alt: labelImg - After selecting image folder

Then specify the directory where you are storing these images' labels. Label directory can be empty, that is the time you start annotating.

.. image:: https://i.imgur.com/x0Dc1Rb.png
     :alt: labelImg - After selecting label folder

Use your mouse to draw or modify the boxes. Use the buttons "Prev Image", "Next Image" to move between images. Almost actions have hotkeys as below:

+------------+--------------------------------------------+
| Ctrl + u   | Load all of the images from a directory    |
+------------+--------------------------------------------+
| Ctrl + r   | Change the default annotation target dir   |
+------------+--------------------------------------------+
| Ctrl + s   | Save                                       |
+------------+--------------------------------------------+
| Ctrl + d   | Copy the current label and rect box        |
+------------+--------------------------------------------+
| Space      | Flag the current image as verified         |
+------------+--------------------------------------------+
| w          | Create a rect box                          |
+------------+--------------------------------------------+
| d          | Next image                                 |
+------------+--------------------------------------------+
| a          | Previous image                             |
+------------+--------------------------------------------+
| del        | Delete the selected rect box               |
+------------+--------------------------------------------+
| Ctrl++     | Zoom in                                    |
+------------+--------------------------------------------+
| Ctrl--     | Zoom out                                   |
+------------+--------------------------------------------+
| ↑→↓←       | Keyboard arrows to move selected rect box  |
+------------+--------------------------------------------+


For more info, go to `tzutalin/labelImg <https://github.com/tzutalin/labelImg>`__ repo.
