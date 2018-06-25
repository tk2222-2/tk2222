# tk2222
カメラ

import cv2

capture = cv2.VideoCapture(0)

while(True):
    ret, frame = capture.read()
    cv2.imshow('frame',frame)
    if cv2.waitKey(1) & 0xFF == ord('q'):
        break

capture.release()
cv2.destroyAllWindows()

＃＃＃　キボードで’１’と’q’を同時押しするまでカメラ画像を取得して表示し続ける。
