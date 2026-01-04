# Gradient256
After searching for a while, i couldn't find a tool to easily make and use color256 gradients in on my terminal (skill issue?). So i  created Gradient256. An fast, simple and reliable way to make gradients embedded as a library for convenience.

# Installation
For now, you can't instal Gradient256.

# How to use
To import it:
```python
import Gradient256
```

### Making a color gradient 
Making a color gradient is easy, making a 5 colors gradient between white and black simply do:
```python
white-black_gradient = Gradient256.gradient((255,255,255), (0,0,0), 5)
```
Remember, this library only works with RGB-255 max codes. This function will return a list of tuples representing RGB codes.
The output of the code above would look like this:
`[(255, 255, 255), (208, 208, 208), (158, 158, 158), (98, 98, 98), (48, 48, 48)]`

### Applying a color gradient into a string
Applying  a gradient into a string is also an elementary task.
```python
gr-cy=Gradient256.grad_text((0,255,0),(0,255,255),'Easy color gradients. Green - Cyan')
re-ye=Gradient256.grad_text((255,0,0),(255,255,0),'Easy color gradients. Red - Yellow')
bl-wh=Gradient256.grad_text((0,0,255),(255,255,255),'Easy color gradients. Blue White')
```

The resulting output should looks somewhat like this:
[Image will be added soon]

# Development
As it is, the code presented isn't perfect but does the job. In the future i plan to add diretional gradients (vertical, diagonal), support to ASCII art (a way to apply gradients to ASCII art easly), a better and smoother gradient algorithm and much more.

## Special thanks
I would like to thank `@KaasKroket` for helping me with the oklab to rgb converter.