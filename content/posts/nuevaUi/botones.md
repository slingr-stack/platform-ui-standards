## **Buttons**

All buttons will have the same font size, icon size, and color distribution. The only variation will be in length.

- **`sm`**: Border radius 6px, responsive width, height 35px, padding top and bottom 8px
- **`md`**: Border radius 6px, responsive width, height 37px, padding top and bottom 9px
- **`lg`**: Border radius 6px, responsive width, height 40px, padding top and bottom 10.5px

Padding for right and left is 13px, and the margin between icon and text is 5px.

### Order of Priority
It is important to remember that priority is taken from **left** to **right**; that is, the first priority is on the left and the last priority is on the right.

- **`First Priority`**: ‘createButton’, ‘deleteButton’, ‘saveButton’
- **`Second Priority`**: ‘editButton’, ‘applyButton’, ‘createAndEditButton’
- **`Third Priority`**: ‘refreshButton’, ‘importButton’, ‘exportButton’, ‘orderUpButton’, ‘orderDownButton’
- **`Last Priority`**: ‘cancelButton’, ‘resetButton’
