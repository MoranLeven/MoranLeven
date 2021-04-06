### Hi there 👋

### Too Busy Doin Nothin 😎

``` python
$ sudo su 
# (▀̿Ĺ̯▀̿ ̿)
import cv2
cam = cv2.VideoCapture(0)
cam.set(3,1920)
cam.set(4,1080)
cam.set(15,-18)
# cam.set(10,200)
while True:
    ret, frame = cam.read()
    cv2.imshow('camera',frame)
    if cv2.waitKey(340) & 0xff == ord('q'):
        break
cam.release()
cv2.destroyAllWindows()
```

