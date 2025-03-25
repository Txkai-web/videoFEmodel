# videoFEmodel
端口说明：增加人脸检测和关键点提取的操作，实现视频的宏表情检测，每0.5秒输出帧图片和帧宏表情结果

端口地址http://localhost:5000/Analyze-Video
传入操作post

输出说明：执行post操作后会生成temp_frames文件夹用于存放帧图片（2FPS)
		图片命名为frame_0.5.png、frame_1.0.png...... 分别代表视频第0.5秒的图片，视频第1秒的图片

注意事项：haarcascade_frontalface_alt.xml文件和LibreFace_FE.onnx都必须放在exe文件相同目录下
		haarcascade_frontalface_alt.xml 是一个用于人脸检测的预训练级联分类器文件，与 OpenCV 库一起使用。它是基于 Haar 特征的分类器，用于在图像或视频中检测人脸。
		LibreFace_FE.onnx 是用于从人脸图像中提取表情特征的模型。
