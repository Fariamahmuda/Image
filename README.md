# Image
ImageArithmaticwithOpencv
Python · plantsImage




import cv2
import matplotlib.pyplot as plt
import numpy as np
import warnings
warnings.filterwarnings('ignore')
%matplotlib inline

def plt_imshow(title,image):
    image = cv2.cvtColor(image,cv2.COLOR_BGR2RGB)
    plt.imshow(image)
    plt.title("plant's Image")
    plt.grid(True)
    plt.show()
    
    
    args = {"image":"../input/plantsimage/20210508_152112.jpg","scharr":0}
#../input/plantsimage
#../input/plantsimage/20210508_152112.jpg

im=cv2.imread(args["image"])
plt.imshow(im)cv2.imread("20210508_152112.jpg")
img=cv2.imread("../input/plantsimage/20210508_152112.jpg")
img.shape

img

len(img)
plt.imshow(img)

imageAddCustomValue=cv2.add(np.uint8([200]), np.uint8([100]))
imageSubractCustomValue=cv2.subtract(np.uint8([50]), np.uint8([100]))
print("Image Maximum Value of 255{}".format(imageAddCustomValue))

import cv2
import matplotlib.pyplot as plt
import numpy as np
import warnings
warnings.filterwarnings('ignore')
%matplotlib inline
def plt_imshow(title,image):
    image = cv2.cvtColor(image,cv2.COLOR_BGR2RGB)
    plt.imshow(image)
    plt.title("plant's Image")
    plt.grid(True)
    plt.show()
args = {"image":"../input/plantsimage/20210508_152112.jpg","scharr":0}
#../input/plantsimage
#../input/plantsimage/20210508_152112.jpg
im=cv2.imread(args["image"])
plt.imshow(im)
<matplotlib.image.AxesImage at 0x7fb1437fa690>

cv2.imread("20210508_152112.jpg")
img=cv2.imread("../input/plantsimage/20210508_152112.jpg")
img.shape
(2240, 4608, 3)
img
array([[[213, 231, 242],
        [214, 232, 243],
        [207, 225, 236],
        ...,
        [146, 168, 163],
        [144, 166, 161],
        [140, 162, 157]],

       [[211, 229, 240],
        [213, 231, 242],
        [207, 225, 236],
        ...,
        [143, 165, 160],
        [143, 165, 160],
        [141, 163, 158]],

       [[207, 225, 236],
        [209, 227, 238],
        [206, 224, 235],
        ...,
        [145, 165, 160],
        [146, 166, 161],
        [147, 167, 162]],

       ...,

       [[197, 185, 175],
        [198, 186, 176],
        [198, 186, 176],
        ...,
        [ 12,  23,  50],
        [ 13,  24,  51],
        [ 13,  24,  51]],

       [[195, 183, 173],
        [196, 184, 174],
        [195, 183, 173],
        ...,
        [ 11,  22,  49],
        [ 10,  21,  48],
        [ 11,  22,  49]],

       [[193, 181, 171],
        [193, 181, 171],
        [191, 179, 169],
        ...,
        [ 10,  21,  48],
        [ 10,  21,  48],
        [ 12,  23,  50]]], dtype=uint8)
len(img)
2240
plt.imshow(img)
<matplotlib.image.AxesImage at 0x7fb141e92dd0>

imageAddCustomValue=cv2.add(np.uint8([200]), np.uint8([100]))
imageSubractCustomValue=cv2.subtract(np.uint8([50]), np.uint8([100]))
print("Image Maximum Value of 255{}".format(imageAddCustomValue))

Image Maximum Value of 255[[255]]
print("Image Minimum Value of 255{}".format(imageSubractCustomValue))

m= np.ones(img.shape, dtype=np.uint8)*100
m

img 

add = cv2.add(img, m)
plt_imshow("Added value", add)

sub = cv2.subtract(img, m)
plt_imshow("Subtructed Value", sub)






