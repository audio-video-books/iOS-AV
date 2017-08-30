# iOS-AV

[iOS视频 裁剪／拼接／压缩（时间维度）](http://veslam.me/2016/07/26/ios-video-clip-combine-compress/)

之前已经实现了个需求是录屏分享，然而如今，野生的新需求出现了，那就是根据用户触发事件的时间点，裁剪/拼接视频。
查了很久资料，得知AVFoundation可用，推荐Apple官方说明文档，十分详细。


[静态和动态媒体采集](http://idup.club/avfoundation_programming_guide:still_and_video_media_capture)

要管理从一个设备（如相机和麦克风）而来的捕获，配置对低昂来代表输入和输出，用一个AVCaptureSession实例整合他们的数据流。你至少需要：  
一个 AVCaptureDevice实例来代表输入设备，例如相机和麦克风  
一个 AVCaptureInput具体子类的实例来配置输入设备接口  
一个 AVCaptureOutput具体子类的实例来管理输出到影片文件还是静态图像  
一个 AVCaptureSession实例来整合从输入到输出的数据流  
