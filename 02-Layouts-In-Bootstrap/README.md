## 02-Layouts-In-Bootstrap

## 5. Breakpoints in Bootstrap 5

- Media Queries
- Breakpoints are Media Queries
- Building Block of RWD
- Mobile First

### Media Queries

Before we dive into breakpoints, let's understand what are breakpoints if you have ever worked with CSS before, you might have heard about media queries. In media queries, you can define which style to apply based on different device screen size

### Breakpoints are Media Queries

Breakpoints in bootstrap are nothing but predefined media queries with a prebuilt styles and designs. With breakpoints, we can choose which style to apply based on device size

### Building Block of RWD

Breakpoints are the building blocks of responsive web design. We use them to control our website and layout based on viewport and device size

### Mobile First

There are mobile device users than desktop users. This raises the question is your website compatible with mobile devices? If not, you're losing a lot of visitors to your website. This is why Bootstrap has made its framework the mobile first CSS framework

There are more than thousands of devices that have web access. It's almost impossible for us to identify all of the device sizes and make websites for specific devices. This is where Bootstrap comes in.

Bootstrap has six breakpoints, starting from device width, which is less than 576 pixels to more than 1400 pixels. Visually, all smaller mobile devices with basic web access to full blown large screen TVs. Bootstrap sites can be accessed anywhere on any device.

All this is possible with the help of breakpoints. Let's have a closer look at how these breakpints work.

Bootstrap is a mobile first framework, this means if you create a UI without any classes at all, Bootstrap will automatically apply mobile compatibility to your web page.

| No. | Class Name |       Break Point | Dimensions |
| --- | :--------: | ----------------: | ---------: |
| 1.  |    None    |       Extra Small |    < 576px |
| 2.  |     sm     |             Small |   >= 576px |
| 3.  |     md     |            Medium |   >= 768px |
| 4.  |     lg     |             Large |   >= 992px |
| 5.  |     xl     |       Extra Large |  >= 1200px |
| 6.  |    xxl     | Extra Extra Large |  >= 1400px |

- Extra Small: Device width for this is less than 576 pixels.
- Small: Device screens that are greater than or equal to 576 pixels, these devices are usually mobile devices like your smartphones
- Medium: Any device with a screen width of 768 pixels or greater than, usually tablet computers, small scale laptops or any portable device with 8 to 10 inch screens
- Large: Large devices with display size of 992 pixeles, or greater than that, these devices are usually your laptop screen sizes of 14 to 15 inches or desktop devices with 18 inch screen sizes and sometimes for than that
- Extra Large: For devies with a screen width of 1200 pixeles or greater than that, like PC monitors or sometimes TV screens too
- Extra Extra Large: For devies with a screen width of 1400 pixeles, like 4k monitors

## 6. Containers

When we build our web components, we want them to be in a specific content holder, this content holder is what's called a container. When you're using a default grid system, containers come very handy.

By default, bootstrap comes with 3 different containers

- .container
  - By using just a container, we set the max width for each breakpoint in the grid system
- .container-{breakpoint}
  - When we use the container with a breakpoint like SM or MD they are specified for that breakpoint. But if the breakpoint is not specified, they are by default set to 100%
- .container-fluid
  - When we use the fluid extension, the web remains 100% on all the breakpoints

### Container Sizes

|                  | Extra Small | Small | Medium | Large | X-Large | XX-Large |
| ---------------- | :---------: | ----: | -----: | ----: | ------: | -------: |
| .container       |    100%     | 540px |  720px | 960px |  1140px |   1320px |
| .container-sm    |    100%     | 540px |  720px | 960px |  1140px |   1320px |
| .container-md    |    100%     |  100% |  720px | 960px |  1140px |   1320px |
| .container-lg    |    100%     |  100% |   100% | 960px |  1140px |   1320px |
| .container-xl    |    100%     |  100% |   100% |  100% |  1140px |   1320px |
| .container-xxl   |    100%     |  100% |   100% |  100% |    100% |   1320px |
| .container-fluid |    100%     |  100% |   100% |  100% |    100% |     100% |

## 7. Grid

### folder-01

### index.html

Bootstrap uses containers, rows and columns just like spreadsheet to create any kind of layout we need.

The grid sistem will extend based on your column specification, but rows can
hold up to 12 columns. One thing we need to understand here is that rows are
wrappers for columns and the container is the parent holder for those rows and columns

### resize-html

What we're trying to accomplish here is that we want the first column
to be only 75% width and the second column the width of 25%

Now you can see there is some space between these columns, The spacing is called Gutter. Usually columns have Gutter sizing on the left and the right sides

Now, if you inspect the core element in the dev tools, you can see that we have some spacing on the right and left that's the gutter width. Bootstrap gives the possibility to customize the gutter width and gutter size too.

### Removing gutter size

```
// Let's say i don't want any gutter sizing on my columns
// add the g-0
<div class="col-8 g-0">
    <div class="bg-primary text-white p-3">
        Columns
    </div>
</div>
```

### Adding gutter size

Let's try adding some gutter size, it's a bit tricky, you can't simply add gutter 2 or 3, this will add the gutter size for all the sides except for the bottom of the column

We can add gutter size separately using a special class called

- gx is used to give size to the left and right
- gy to the top

```
<div class="col-8 gy-3">
    <div class="bg-primary text-white p-3">
        Columns
    </div>
</div>
<div class="col-4 gx-3">
    <div class="bg-primary text-white p-3">
        Columns
    </div>
</div>
```

## 8. Grid Options

### grid-options-html

**Bootstrap grid system has its options**

What i need now is that the breakpoint for MD medium devices is meet, i want the
columns to break into 4 divisions, but when the breakpoint reaches the small width or SM breakpoint, i want all the columns in a single row or disabled **col-md-3 or medium device has a breakpoint on 768px**

```
<div class="container">
    <div class="row">
        <div class="col-md-3">
            <div class="bg-primary p-3 text-white text-center">
                Columns
            </div>
        </div>
        <!-- ..... -->
        <!-- repeat this col-md-3 a total of four times -->
    </div>
</div>
```

Let's try other breakpoints, What i want now is that when i reach the MD breakpoint or the medium screen device, what that is 768px i want all the columns to be divided in 3 columns

The way to work with columns is to simply divide them by the number of columns you need. For example, now i need three columns, so let's divide 12 / 3 = 4 , **col-sm-4**

```
<div class="container">
    <div class="row">
        <div class="col-md-3 col-sm-4">
          <div class="bg-primary p-3 text-white text-center mb-3">
            Columns
          </div>
        </div>
        <!-- ..... -->
        <!-- repeat this col-md-3 col-sm-4 a total of four times -->
    </div>
</div>
```

## 9. Nesting Rows and Columns

### nesting-rows-columns-html

Remember, if you want to nest columns within columns, you should always use rows in the child element, This will give you a proper output.

## 10. Column Vertical Alignment

### column-vertical-alignment-html

Let's see how we can customize our columns for better usability

```
<div class="align-items-start">
<div class="align-items-center">
<div class="align-items-end">
```

Next in the vertical alignment, we have another class called self. Here the columns will align automatically based on the height of the row.

## 11. Column Horizontal Alignment

### column-horizontal-alignment-html

Let's see how we can align columns horizontally for

## 12. Column Wrapping and Column Breaks

### column-wrapping-column-breaks-html

As we know, a row can hold up to 12 columns, but what if we specified more than that? let's say that we specified 13 columns, so let's see what happens.

Usually when you want to break a list of columns, you would use them in a new row. That would create a new row of columns, but we don't have to do that anymore. Instead, we can use then W 100 class, which adds a 100% width.

## 13. Reordering and Offsetting Columns

### reordering-offsetting-columns-html

There will be times when you would want to move a column to a different location in that row. But since the columns work from left to right, you might find it a little bit difficult to work with that. This is where the ordering classes come in, You'll be able to control the visual order of your columns with reordering, here you can use the dot order class to get your job done.

Let's try **reordering** them, What we are trying to accomplish here is that we want the first column to be the last and the last column to be the first and rearrange every other columns to.

**Offsetting** is a little different than reordering, here we are not just reordering the columns, but we are also moving them from one place to another

Let's say that i want to move a column to the right, here to move a column to the right we use the offset class, what this does is that it increases the left margin of a column from other columns.

## 14. Margin Utilities

### margin-utilities-html

In the last lecture, we saw how to apply margin left with offset class, But what if you want to add right margin as well? This is where the modern utilities come into action

Here we have two columns and what i want to make is that the second column move to the right, we have already saw that with the offset class, but let's see how we can do that with the margin classes.

```
<div class="container">
    <div class="row h-10 bg-info">
        <div class="col-md-3">
            <div class="bg-primary p-3 mt-3 text-white">
            1st Column
            </div>
        </div>
        <div class="col-md-3 ms-auto">
            <div class="bg-primary p-3 mt-3 text-white">
            2nd Column
            </div>
        </div>
    </div>
</div>
```

We already saw that one in the last class, Let's see how we can apply the same margin style to the first column, for that all we have to do is instead of using the **ms-auto** on the second column, we will use the **me-auto** on the first column

## 15. Gutters

- Gutters are Gabs between columns
- Padding Right and Left
- Gutters start at 1.5rem(24px) wide
- Gutters can be adjusted

When we are working with grid system and columns you will see gaps between these columns. These gaps are called **Gutters**, these are padding between columns, they are used to space and align contents responsively in bootstrap grid system

These patterns are horizontal, usually set by **padding left and right** on each column, and we use the offset method which uses a negative margin to move the column

The size of the **Gutters** is 1.5rem, which is 24px, which works well with the grid system

Gutters can be ajusted based on the breakpoint specific classes we can modify horizontal gutters, vertical gutters and all gutters

## 16. Horizontal Gutters

### horizontal-gutters-html

To apply the horizontal gutter size, we use the gx class, but when we apply the gx for the row, it may overflow the container, so if you come across such an issue, make sure to use the px class on the container, the px applies padding on the x axis of the container.

`<div class="row mb-3 bg-warning h-10 gx-5">`

If you check your browser on our example, you can see that the row is overflowing just as we thought, this added the padding for a row, which increases the size of the row to flow outside the container.

```
<div class="container bg-info mt-5 px-4">
```

There is another way how we can fix the container overflow problem, this is with the help of another class called **overflow-hidden**. We have to apply this class to the container to fix the overflow issue

## 17. Vertical Gutters

### vertical-gutters-html

The only difference here is the class name and sort of using **gx-5**, now we'll be using **gy-5**. Here g is the gutter and y is the they y axis and 5 is the measurement we want to apply, to avoid overflow we will use **overflow-hidden** class on the container

## 18. Horizontal and Vertical Gutters

### horizontal-vertical-gutters-html

In this class we will see how we can use a single class name to apply both horizontal and vertical gutters sizing

There are times when you will want to apply gutter sizing based on a breakpoint, For example, you want a g-5 sizing on md breakpoint and g-3 sizing on sm breakpoint. You can accomplish that by using a class called gmd-5 for md breakpoints and gsm-3 for sm breakpoints

## 19. Quiz 2: Section 2

### Question 1: Check the available breakpoints in Bootstrap 5.2?
- [ ] - Extra Small
- [ ] - Small
- [ ] - Medium
- [ ] - Large
- [ ] - Extra Large
- [ ] - Extra Extra Large
- [X] - All of the above

### Question 2: What’s required when using default grid system in Bootstrap?
- [X] - Container
- [ ] - JQuery
- [ ] - Plug-ins
- [ ] - None of the above

### Question 3: Twelve column Grid System is used in Bootstrap’s grid system?
- [X] - True
- [ ] - False

### Question 4: You can use vertical and horizontal alignments on Bootstrap columns?
- [X] - True
- [ ] - False

### Question 5: Bootstrap columns cannot be re-arranged?
- [ ] - True
- [X] - False

### Question 6: What do offset classes do?
- [ ] - Increase the left padding
- [ ] - Decrease the right padding
- [X] - Increase the left margin
- [ ] - None of the above

### Question 7: What are gutters?
- [X] - Padding between the columns
- [ ] - Margin between the columns
- [ ] - Colors in Bootstrap
- [ ] - None of the above