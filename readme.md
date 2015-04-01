# 애니메이션 GIF를 안드로이드에서 인코딩할 수 있는 라이브러리.
# Animated gif encoder for android.

j2me 버전으로 만들어진 Animated GIF encoder 를 수정해서 android 에서 돌릴 수 있도록 했음.
( Original j2me version : http://www.jappit.com/blog/2008/12/04/j2me-animated-gif-encoder/ )


* 사용 방법 (How to use).
```java
 ByteArrayOutputStream bos = new ByteArrayOutputStream();
  
 AnimatedGifEncoder encoder = new AnimatedGifEncoder();
 encoder.start(bos);
 encoder.addFrame(image1);
 encoder.addFrame(image2);
 encoder.finish();
  
 return bos.toByteArray();
```
image1과 image2는 android.graphics.Bitmap의 인스턴스임 (image1 and image2 is android.graphics.Bitmap).
