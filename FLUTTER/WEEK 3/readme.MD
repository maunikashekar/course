# FLUTTER

## WEEK 3

### WIDGETS

#### TEXT WIDGET

The Text widget allows you to create a styled text in your application.

#### CONTAINER WIDGET

The Container widget allows to create a rectangular visual element. A container has properties, such as a background, a border, or a shadow. A Container can also have margins, padding, and constraints applied to its size.

#### APPBAR WIDGET

The AppBar widget creates a Container with a height of 56 device-independent pixels with an internal padding of 8 pixels, both on the left and the right. Inside the container, AppBar uses a Row layout to organize its children. The middle child, the title widget, is marked as Expanded, which means it expands to fill any remaining available space that hasn’t been consumed by the other children. You can have multiple Expanded children and determine the ratio in which they consume the available space.

#### SCAFFOLD WIDGET

The Scaffold widget organizes its children in a vertical column. At the top of the column it places an instance of AppBar, passing the app bar a Text widget to use as its title. Passing widgets as arguments to other widgets is a powerful technique that lets you create generic widgets that can be reused in a wide variety of ways. Finally, Scaffold uses an Expanded to fill the remaining space with its body, which consists of a centered message.
