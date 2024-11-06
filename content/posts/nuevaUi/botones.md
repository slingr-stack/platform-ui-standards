### Button Standards

All buttons in the new UI should follow a uniform style for font size, icon size, and color distribution. The only permitted variation is in button length. 

#### Button Sizes
- **Small (sm)**: Border radius 6px, responsive width, height 35px, padding top and bottom 8px
- **Medium (md)**: Border radius 6px, responsive width, height 37px, padding top and bottom 9px
- **Large (lg)**: Border radius 6px, responsive width, height 40px, padding top and bottom 10.5px
- **Padding (left and right)**: 13px for all sizes
- **Icon and Text Spacing**: 5px margin between icon and text

#### Button Priority Order
Button priority should follow a **left-to-right** arrangement, with higher-priority actions on the left and lower-priority actions on the right.

1. **First Priority**: `createButton`, `deleteButton`, `saveButton`
2. **Second Priority**: `editButton`, `applyButton`, `createAndEditButton`
3. **Third Priority**: `refreshButton`, `importButton`, `exportButton`, `orderUpButton`, `orderDownButton`
4. **Last Priority**: `cancelButton`, `resetButton`

*Note:* Ensure that buttons are ordered logically to guide users in understanding action priorities.

