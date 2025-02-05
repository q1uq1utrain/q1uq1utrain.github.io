# q1uq1utrain.github.io
import random
from math import sin, cos, pi, log
from tkinter import *

CANVAS_WIDTH = 980
CANVAS_HEIGHT = 720
CANVAS_CENTER_X = CANVAS_WIDTH / 2
CANVAS_CENTER_Y = CANVAS_HEIGHT / 2
IMAGE_ENLARGE = 11

HEART_COLOR_LIST = ["#d974ff"]

def heart_function(t, shrink_ratio: float = IMAGE_ENLARGE):
    """
    create a heart
    : param shrink_ratio: ratio
    :param t: parameter
    :return: x, y
    """
    x = 16 * (sin(t) ** 3)
    y = -(13 * cos(t) - 5 * cos(2 * t) - 2 * cos(3 * t) - cos(4 * t))

    x *= shrink_ratio
    y *= shrink_ratio
