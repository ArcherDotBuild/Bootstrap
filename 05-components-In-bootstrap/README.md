## 05-Components-In-Bootstrap

## 38. Accordions

## 39. Alerts

## 40. Dismissing Alerts

## 41. Badges

Badges are inline styled elements which you can use anywhere,
like heading tags and paragraphs. Badges look like a small button
but are not actually buttons, Badges can be scaled to match your DOM
element. For example, if you use a badge and h1 tag, it would inherit
the size of an h1 and if you use it in a paragraph tag, it would inherit
the size of a paragraph. Also in Bootstrap 5, badges have no longer
have focus or hover styles for links.

## 42. Breadcrumb

Breadcrumbs are a way to show the current page location to the user.
Bootstrap helps in adding an automatic separator for each page with
the help of CSS

### Entity

An HTML entity is a piece of text ("string") that begins with an ampersand (&) and ends with a semicolon (;). Entities are frequently used to display reserved characters (which would otherwise be interpreted as HTML code), and invisible characters (like non-breaking spaces). You can also use them in place of other characters that are difficult to type with a standard keyboard.  
https://developer.mozilla.org/en-US/docs/Glossary/Entity

https://html.spec.whatwg.org/multipage/named-characters.html#named-character-references

## 43. Buttons

## 44. Button Group

## 45. Button Toolbar

## 46. Button Group Alteration

## 47. Card

## 48. Card Sizing

## 49. Card Navigation

## 50. Card Images

## 51. Card Styles

## 52. Carousel

## 53. Carousel Controls

## 54. Carousel Indicators

## 55. Carousel Caption file21

## 56. Carousel Fade Effect file21

## 57. Carousel Timing

## 58. Disable Carousel Touch Swiping

## 59. Carousel Dark Variant

## 60. Close Button

## 61. Collapse

## 62. Horizontal Collapse

## 63. Multiple Targets

## 64. Dropdowns

## 65. Split Button

## 66. Dropdown Sizing file32

## 67. Dark Dropdowns file32

## 68. Dropdown Directions

## 69. Dropup and Dropdown Alignment

## 70. Menu Items

## 71. Menu Alignment

## 72. Dropdown Alignment Options

## 73. Menu Contents

## 74. Dropdown Forms

## 75. Dropdown Options

## 76. Dropdown Auto Close

## 77. List Group

## 78. List Group Links and Buttons file43

## 79. List Group Flush file43

## 80. Numbered List

## 81. Horizontal List Groups

## 82. Contextual List Group Classes

## 83. List Group with Badges

## 84. List Group with Custom Content

## 85. List Group Checkboxes and Radios

## 86. List Group JavaScript Tabs

## 87. Modals

- Built with HTML, CSS, and JavaScript
- Positioned on Top of Everything Else
- 1 Modal support at a Time
- Nested Modals are not supported
- Positioned to fixed by default

It's a JavaScript plugin that's built into bootstrap, with the help of modals, you can create dialogs, light boxes, user notifications and so much more. Some things you should note before getting started with modals are that modals are built with HTML, CSS and JavaScript

## 88. Static Backdrop

## 89. Scrolling Long Content

## 90. Vertically Centered

## 91. Modal Tooltips and Popovers

## 92. Using Grid System In Modal

## 93. Varying Modal Content

## 94. Toggle Between Modals

## 95. Optional Modal Sizes

```
class="modal fade modal-sm"
class="modal fade modal-lg"
class="modal-dialog modal-fullscreen

Fullscreen on mobile devices
class="modal-dialog modal-fullscreen-sm-down"
```

## 96. Navbar

## 97. Navigation Links

## 98. Navbar Dropdown

## 99. Navbar Nested Dropdown

## 100. Navbar Forms

## 101. Navbar Input Group

## 102. Navbar Plain Text

## 103. Navbar Colors

## 104. Navbar Containers

## 105. Navbar Placement

```
<nav class="navbar bg-light fixed-top">
<nav class="navbar bg-light fixed-bottom">

// Sticks when touches the top
<nav class="navbar bg-light sticky-top">

// Sticks until the navigation reaches
<nav class="navbar bg-light sticky-top">
```

## 106. Navbar Scrolling

## 107. Off Canvas Navbar

## 108. Navs and Tabs

## 109. Nav Flex Utilities

## 110. Nav Tabs and Pills with Dropdown

## 111. Tabs and Pills Behaviors

## 112. Offcanvas In-Depth

## 113. Offcanvas Scrolling

```
data-bs-backdrop="true"
data-bs-backdrop="false"
data-bs-backdrop="static"
```

## 114. Offcanvas Placement

```
class="offcanvas offcanvas-start"
class="offcanvas offcanvas-end"
class="offcanvas offcanvas-top"
class="offcanvas offcanvas-bottom"

```

## 115. Pagination

## 116. Placeholders

## 117. Popovers In-Depth

## Popovers

- Rely on 3rd Party Library
- Require Popover Plug/in
- Requires Manual Initialization

## 118. Popover Direction

## 119. Custom Popovers file83

## 120. Dismiss on Next Click file83

## 121. Enable Popover On Hover file83

`data-bs-trigger="focus"`
`data-bs-trigger="hover focus"`

## 122. Progress Bars

## 123. Progress Bar Height and Background

## 124. Stripes And Animation

## 125. Scrollspy

## 126. Spinners

## 127. Growing Spinner

## 128. Spinner Alignment

## 129. Spinner Sizes

## 130. Spinner In Buttons

## 131. Toasts

## 132. Toast Alignment

```
// top and left
class="toast position-fixed text-bg-primary top-0 start-0 ms-3 mt-3"
// top and right
class="toast position-fixed text-bg-primary top-0 end-0 me-3 mt-3"
// bottom and right
class="toast position-fixed text-bg-primary bottom-0 end-0 me-3 mb-3"
// bottom and left
class="toast position-fixed text-bg-primary bottom-0 start-0 ms-3 mb-3"
```

## 133. Tooltips In-Depth

## 134. Custom Tooltip

## 135. Tooltip Directions

## 136. Html in Tooltip

## 137. Tooltip On Disabled Elements

## Quiz 5: Section 5

### Question 1: Accordion is not a JavaScript plug-in in Bootstrap?

- [ ] - True
- [x] - False

### Question 2: Alerts can be used with contextual classes to apply background color and font color?

- [x] - True
- [ ] - False

### Question 3: Badges can be used inside buttons?

- [x] - True
- [ ] - False

### Question 4: Dividers in breadcrumb cannot be modified?

- [ ] - True
- [x] - False

### Question 5: You can disable a button with a attribute called?

- [ ] - disable
- [x] - disabled
- [ ] - class="disable-button"
- [ ] - class="deactivate"

### Question 6: You can group the buttons, with a class called?

- [ ] - group-btn
- [x] - btn-group
- [ ] - btn-set
- [ ] - btn-group-set

### Question 7: You can use contextual classes with btn-group to change the color of individual buttons?

- [x] - True
- [ ] - False

### Question 8: You can group radio buttons?

- [x] - True
- [ ] - False

### Question 9: You can change the size of the card with the class?

- [ ] - card-sm
- [ ] - card-lg
- [ ] - card-big
- [x] - None of the above

### Question 10: Dark mode is available for Bootstrap carousel?

- [x] - True
- [ ] - False

### Question 11: You need a class called close-btn to get the close button?

- [ ] - True
- [x] - False

### Question 12: .collapse.show is used to show the content in collapsible panel?

- [x] - True
- [ ] - False

### Question 13: Split button requires a class called?

- [ ] - dropdown-split
- [ ] - split-dropdown
- [x] - dropdown-toggle-split
- [ ] - split-toggle-dropdown

### Question 14: You can create list groups with the class?

- [x] - list-group
- [ ] - group-list
- [ ] - list-grouped
- [ ] - grouped-list

### Question 15: When backdrop is set to static, the modal will not close when clicked outside of it

- [x] - True
- [ ] - False

### Question 16: You cannot include search field in NavBar?

- [ ] - True
- [x] - False

### Question 17: To create vertical navbar, we use the class called?

- [ ] - vertical-navbar
- [ ] - navbar-vertical
- [x] - flex-column
- [ ] - column-flex

### Question 18: data-bs-backdrop="static" is used to set backdrop to static in Offcanvas?

- [x] - True
- [ ] - False

### Question 19: You can use icons in pagination?

- [x] - True
- [ ] - False

### Question 20: placeholder-glow gives glowing effect on placeholder?

- [x] - True
- [ ] - False

### Question 21: You must initialize popovers before they can be used?

- [x] - True
- [ ] - False

### Question 22: To create striped progress bar, you need to use the class called?

- [ ] - progress-bar-stripe
- [x] - progress-bar-striped
- [ ] - progress-bar
- [ ] - striped-progress-bar

### Question 23: Scrollspy automatically updates Bootstrap navigation?

- [x] - True
- [ ] - False

### Question 24: Bootstrap Spinners use JavaScript to rotate?

- [ ] - True
- [x] - False

### Question 25: Toasts can be aligned anywhere in the viewport edges?

- [x] - True
- [ ] - False

### Question 26: Tooltips can be set to 4 different directions?

- [x] - True
- [ ] - False
