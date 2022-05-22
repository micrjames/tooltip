# tooltip
A multi-directional tooltip.

## Table Of Contents
* [General Info](#general-info)
* [Technologies Used](#technologies-used)
* [Features](#features)
* [Setup](#setup)
* [Usage](#usage)
* [Project Status](#project-status)
* [Room for Improvement](#room-for-improvement)
* [Contact](#contact)

## General Info
This project entails an example of a generalized tooltip in multiple directions.
## Technologies Used
This project is created using:
* SCSS - Used to programmatically alter the orientations of the arrow tip and the displacement of the area containing the text.
## Features
The Tooltip Component allows configuration of text and tooltip text, as in the below examples where text is set to be "some text" and the tooltip text is set to display "some tooltip text." Furthermore, the orientation of the arrow tip and displacement of the area containing the text can be configured to any combination of upper and lower and center, left, and right.
## Setup
Just download the scss folder and import the _tooltip.scss file to the scss file you are using in your project. Assuming that the tooltip scss file is in the same directory as the scss file for your project, import _tooltip.scss like this:
```
@import './tooltip';
```
## Usage
Include the mixin from the tooltip mixin code file to your project like this (to specify a default tooltip):
```
.tooltip {
		...
    // code defining the style of your tooltip
	  @include tooltip($font-size, $background-color, $text-color);
}
```
To specify a non-default tooltip, change the argument values in the mixin:
```
tooltip($font-size, $background-color, $text-color, $direction, $justify, $displacement)
```
The arguments font-size, background-color and text-color are obvious in what they do. The value of the direction specifies whether the tooltip is to be displayed *above* or *below* the parent element to which the tooltip is attached. The value of the justify argument specifies whether the arrow tip of the tooltip is displayed to the *right*, *left* or *center* of the tooltip. The value of the displacement specifies whether the container of the tooltip will be displaced to the *left* or *right* of where the container would normally be. A value of *null* applied to the displacement argument specifies that the displacement of the container should not be changed.
## Project Status
This project will remain in production until such time as I no longer need to update the tooltip to accomodate any project for which I may have the need.
## Room for Improvement
As indicated in the Project Status section, the need may arise so that the tooltip may need to adjusted for some particular project.
## Contact
Feel free to contact me @michaelrjamesjr on twitter or on github @micrjames or check out my blog at michaelrjames.hashnode.dev
