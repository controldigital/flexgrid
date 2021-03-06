Flexgrid.css
========
Flexbox based 12-column grid build specially build for Control sites to replace the Bootstrap grid.
The grid is based on the Bootstrap system, but utilizes much more controls that Flexbox brings.

- Author: Control
- Version: 1.3.1
- License: Licensed under the MIT/X11 License (http://opensource.org/licenses/MIT)


## Container
To keep the content inside the grid we use the container class: `.container` or `.container-full`.
By default the `.container` is set to a max-width of `71.25em` or `1140px`. This can be modified by defining your own `.container` class.

```html
<div class="container">
  ...
</div>
```
For a full width page without a grid use `.container-full` which stretches to `100%` of the page width.
```html
<div class="container-full">
  ...
</div>
```

## Row
Rows are the containers that will hold all the columns. `.row` operates as a Flexbox container that is able to position its children on a horizontal axis.

```html
<div class="row">
  ...
</div>
```

### Column
Columns are the same as rows but vertical. They can be set instead of `.row` with `.column`. All the alignments are done on a vertical axis with `.column` present.

```html
<div class="column">
  ...
</div>
```

### Creating rows and columns, and modifying them
The rows have some standard properties. They wrap automatically and have a horizontal direction by default. There are some classes to overwrite this.

| 0px and above             | 768px and above              | 992px and above              | State            |
| ------------------------- | ---------------------------- | ---------------------------- | ---------------- |
| .row                      | .row-sm                      | .row-md                      | Row              |
| .row-reverse              | .row-reverse-sm              | .row-reverse-md              | Row Reversed     |
| .column                   | .column-sm                   | .column-md                   | Column           |
| .column-reverse           | .column-reverse-sm           | .column-reverse-md           | Column Reversed  |
| .wrap                     | .wrap-sm                     | .wrap-md                     | Wrap             |
| .wrap-reverse             | .wrap-reverse-sm             | .wrap-reverse-md             | Wrap Reverse     |
| .nowrap                   | .nowrap-sm                   | .nowrap-md                   | No Wrap          |

### Aligning within rows
Because `.row` is a Flexbox container it is capable of aligning its children. The default alignment value of a Flexbox container is `align-items: stretch`.
By adding classes to the row we are able to change this alignment.

### Axis
Flexbox alignment works on axes. It consists of 2 axes called the `Main axis` and the `Cross axis`. When the row is set to a horizontal direction (**row**) the Y axis is considered the Main Axis and the X axis the Cross axis. When a row is set to a vertical direction (**column**) the X axis is the Main axis and the Y axis the Cross axis.

#### Main axis alignment
The classes below utilize the Flebox property `align-items` and `align-content` which places the children on a given position on the Main axis. `align-items` aligns the children relative to the children on the same row, where `align-content` aligns the children when wrapped in relation to container.

| 0px and above        | 768px and above         | 992px and above         | Alignment  | Axis  |
| -------------------- | ----------------------- | ----------------------- | ---------- | ----- |
| .items-start         | .items-start-sm         | .items-start-md         | Start      | Main  |
| .items-end           | .items-end-sm           | .items-end-md           | End        | Main  |
| .items-center        | .items-center-sm        | .items-center-md        | Center     | Main  |
| .items-baseline      | .items-baseline-sm      | .items-baseline-md      | Baseline   | Main  |
| .items-stretch       | .items-stretch-sm       | .items-stretch-md       | Stretch    | Main  |

| 0px and above        | 768px and above         | 992px and above         | Alignment  | Axis  |
| -------------------- | ----------------------- | ----------------------- | ---------- | ----- |
| .content-start       | .content-start-sm       | .content-start-md       | Start      | Main  |
| .content-end         | .content-end-sm         | .content-end-md         | End        | Main  |
| .content-center      | .content-center-sm      | .content-center-md      | Center     | Main  |
| .content-around      | .content-around-sm      | .content-around-md      | Around     | Main  |
| .content-between     | .content-between-sm     | .content-between-md     | Between    | Main  |


#### Cross axis alignment
The classes below utilize the Flebox property `justify-content` which places the children on a given position on the Cross axis.

| 0px and above        | 768px and above         | 992px and above         | Alignment  | Axis   |
| -------------------- | ----------------------- | ----------------------- | ---------- | ------ |
| .justify-start       | .justify-start-sm       | .justify-start-md       | Start      | Cross  |
| .justify-end         | .justify-end-sm         | .justify-end-md         | End        | Cross  |
| .justify-center      | .justify-center-sm      | .justify-center-md      | Center     | Cross  |
| .justify-around      | .justify-around-sm      | .justify-around-md      | Around     | Cross  |
| .justify-between     | .justify-between-sm     | .justify-between-md     | Between    | Cross  |
| .justify-evenly      | .justify-evenly-sm      | .justify-evenly-md      | Evenly     | Cross  |


## Box
The boxes are the classes that are placed inside a row which give you the options to divide the content in boxes with a flexible or a fixed size.

### Flexible boxes
| 0px and above   | 768px and above  | 992px and above | Size                                                      |
| --------------- | ---------------  | --------------- | --------------------------------------------------------  |
| .box            | .box-sm.         | .box-md         | All boxes are equal of size                               |
| .box-flex       | .box-sm-flex     | .box-md-flex    | Fills the space left in a row                             |
| .box-flex-1     | .box-sm-flex-1   | .box-md-flex-1  | Fills the space left in a row (1/x) (same as `.box-flex`) |
| .box-flex-2     | .box-sm-flex-2   | .box-md-flex-2  | Fills the space left in a row (2/x)                       |
| .box-flex-3     | .box-sm-flex-3   | .box-md-flex-3  | Fills the space left in a row (3/x)                       |
| .box-flex-4     | .box-sm-flex-4   | .box-md-flex-4  | Fills the space left in a row (4/x)                       |
| .box-flex-5     | .box-sm-flex-5   | .box-md-flex-5  | Fills the space left in a row (5/x)                       |
| .box-flex-6     | .box-sm-flex-6   | .box-md-flex-6  | Fills the space left in a row (6/x)                       |
| .box-flex-7     | .box-sm-flex-7   | .box-md-flex-7  | Fills the space left in a row (7/x)                       |
| .box-flex-8     | .box-sm-flex-8   | .box-md-flex-8  | Fills the space left in a row (8/x)                       |
| .box-flex-9     | .box-sm-flex-9   | .box-md-flex-9  | Fills the space left in a row (9/x)                       |
| .box-flex-10    | .box-sm-flex-10  | .box-md-flex-10 | Fills the space left in a row (10/x)                      |
| .box-flex-11    | .box-sm-flex-11  | .box-md-flex-11 | Fills the space left in a row (11/x)                      |
| .box-flex-12    | .box-sm-flex-12  | .box-md-flex-12 | Fills the space left in a row (12/x)                      |
| .box-static     | .box-sm-static   | .box-md-static  | Size of own content                                       |

**Example:**

```html
<div class="row">
  <div class="box"></div>
  <div class="box"></div>
  <div class="box"></div>
</div>
```
**Results in:**

```
==.row ==========================================================
|| ------------------- ------------------- ------------------- ||
|| |      .box       | |      .box       | |      .box       | ||
|| ------------------- ------------------- ------------------- ||
=================================================================
```

**Example:**

```html
<div class="row">
  <div class="box-static"></div>
  <div class="box-flex"></div>
</div>
```
**Results in:**

```
==.row ==========================================================
|| ------------------- --------------------------------------- ||
|| |   .box-static   | |              .box-flex              | ||
|| ------------------- --------------------------------------- ||
=================================================================
```

Flexible boxes like `.box-flex`, `.box-flex-1`, `.box-flex-2` and `.box-flex-3` divide the remaining space in proportion. The space left in the row or column is divided by the total of `flex-grow` values of the flexible children. The children then divide the space per flex-grow of the child.

**Example:**
When we have a `.box-flex-2`, a `.box-flex-3` and a `.box-flex-1` the total of flex-grow values is **6**. The remaining space is divided by this total. `.box-flex-2` will get **2/6**, `.box-flex-3` **3/6** and `.box-flex-1` **1/6** of the space available to its own size.

### Fixed boxes
Flexible boxes are fun, but most of the time we need simple fixed structures that don't move. Fixed boxes are comparable with Bootstrap's cols. They gain a percentage of the container's width and move next to each other.

| 0px and above   | 768px and above | 992px and above | Size  |
| --------------- | --------------- | --------------- | ----- |
| .box-1          | .box-sm-1       | .box-md-1       | 1/12  |
| .box-2          | .box-sm-2       | .box-md-2       | 1/6   |
| .box-3          | .box-sm-3       | .box-md-3       | 1/4   |
| .box-4          | .box-sm-4       | .box-md-4       | 1/3   |
| .box-5          | .box-sm-5       | .box-md-5       | 5/12  |
| .box-6          | .box-sm-6       | .box-md-6       | 1/2   |
| .box-7          | .box-sm-7       | .box-md-7       | 7/12  |
| .box-8          | .box-sm-8       | .box-md-8       | 2/3   |
| .box-9          | .box-sm-9       | .box-md-9       | 3/4   |
| .box-10         | .box-sm-10      | .box-md-10      | 5/6   |
| .box-11         | .box-sm-11      | .box-md-11      | 11/12 |
| .box-12         | .box-sm-12      | .box-md-12      | 1/1   |


### Box offsets
Use offsets to move a box to the right with the just the right percentage. They add a left margin to the box.

| 0px and above   | 768px and above   | 992px and above    | Size  |
| --------------- | ----------------- | ------------------ | ----- |
| .box-offset-1   | .box-sm-offset-1  | .box-md-offset-1   | 1/12  |
| .box-offset-2   | .box-sm-offset-2  | .box-md-offset-2   | 1/6   |
| .box-offset-3   | .box-sm-offset-3  | .box-md-offset-3   | 1/4   |
| .box-offset-4   | .box-sm-offset-4  | .box-md-offset-4   | 1/3   |
| .box-offset-5   | .box-sm-offset-5  | .box-md-offset-5   | 5/12  |
| .box-offset-6   | .box-sm-offset-6  | .box-md-offset-6   | 1/2   |
| .box-offset-7   | .box-sm-offset-7  | .box-md-offset-7   | 7/12  |
| .box-offset-8   | .box-sm-offset-8  | .box-md-offset-8   | 2/3   |
| .box-offset-9   | .box-sm-offset-9  | .box-md-offset-9   | 3/4   |
| .box-offset-10  | .box-sm-offset-10 | .box-md-offset-10  | 5/6   |
| .box-offset-11  | .box-sm-offset-11 | .box-md-offset-11  | 11/12 |
| .box-offset-12  | .box-sm-offset-12 | .box-md-offset-12  | 1/1   |

### Box aligning
The aligning style of the row can be overruled per Box. This is done with the `align-self` property of Flexbox. A small hack is to use margins. For example by setting `margin-left: auto;` the box will justify itself to the right on the Cross axis.

| 0px and above        | 768px and above         | 992px and above         | Alignment  | Axis  |
| -------------------- | ----------------------- | ----------------------- | ---------- | ----- |
| .box-start           | .box-sm-start           | .box-md-start           | Start      | Main  |
| .box-end             | .box-sm-end             | .box-md-end             | End        | Main  |
| .box-center          | .box-sm-center          | .box-md-center          | Center     | Main  |
| .box-baseline        | .box-sm-baseline        | .box-md-baseline        | Baseline   | Main  |
| .box-stretch         | .box-sm-stretch         | .box-md-stretch         | Stretch    | Main  |
| .box-to-top          | .box-sm-to-top          | .box-md-to-top          | Top        | Cross |
| .box-to-right        | .box-sm-to-right        | .box-md-to-right        | Right      | Cross |
| .box-to-bottom       | .box-sm-to-bottom       | .box-md-to-bottom       | Bottom     | Cross |
| .box-to-left         | .box-sm-to-left         | .box-md-to-left         | Left       | Cross |
| .box-to-center       | .box-sm-to-center       | .box-md-to-center       | Center     | Cross |

### Box Order
Flexbox has the cool capability to reorder children of the container. This is done through the `order` property.

| 0px and above          | 768px and above           | 992px and above           | Order        |
| ---------------------- | ------------------------- | ------------------------- | ------------ |
| .box-order-first       | .box-sm-order-first       | .box-md-order-first       | First **-1** |
| .box-order-middle      | .box-sm-order-middle      | .box-md-order-middle      | Middle **0** |
| .box-order-last        | .box-sm-order-last        | .box-md-order-last        | Last **1**   |

### Utilities
Boxes can be hidden and shown based on device with these utility classes. Almost all of the display properties are includes, except for `table` and the new `grid`.

| 0px and above          | 768px and above           | 992px and above           | Display      |
| ---------------------- | ------------------------- | ------------------------- | ------------ |
| .box-hide              | .box-sm-hide              | .box-md-hide              | None         |
| .box-show              | .box-sm-show              | .box-md-show              | Block        |
| .box-show-inline       | .box-sm-show-inline       | .box-md-show-inline       | Inline       |
| .box-show-inline-block | .box-sm-show-inline-block | .box-md-show-inline-block | Inline Block |
| .box-show-flex         | .box-sm-show-flex         | .box-md-show-flex         | Flex         |
| .box-show-inline-flex  | .box-sm-show-inline-flex  | .box-md-show-inline-flex  | Inline Flex  |

## Contact
To report bugs or ask questions, please e-mail the developer [Emiel](mailto:emiel@controldigital.nl)
