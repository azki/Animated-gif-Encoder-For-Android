# 애니메이션 GIF를 안드로이드에서 인코딩할 수 있는 라이브러리.

j2me 버전으로 만들어진 Animated GIF encoder(http://www.jappit.com/blog/2008/12/04/j2me-animated-gif-encoder/)가 있길래 내가 살짝 수정해서 android 에서 돌릴 수 있도록 했음.

* 사용 방법.
```java
 ByteArrayOutputStream bos = new ByteArrayOutputStream();
  
 AnimatedGifEncoder encoder = new AnimatedGifEncoder();
 encoder.start(bos);
 encoder.addFrame(image1);
 encoder.addFrame(image2);
 encoder.finish();
  
 return bos.toByteArray();
```
image1과 image2는 android.graphics.Bitmap의 인스턴스임.
