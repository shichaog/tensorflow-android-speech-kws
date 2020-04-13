# tensorflow-android-speech-kws
A demo of android key word spoting based on tensorflow tutial example.

This is a very good example of using tensorflow in android APP. This example contains only keyword spoting.

The directory speech_commands  is get

To train the model:
python tensorflow/examples/speech_commands/train.py --wanted_words=house


To freeze pb:
python tensorflow/examples/speech_commands/freeze.py --start_checkpoint=/tmp/speech_commands_train/conv.ckpt-18000 --out_file=/tmp/my_frozen_graph.pb ----wanted_words=house

After pb file generated, move to assets directory of android, android directory is an android studio project. The file used by my project is conv_actions_house_labels.txt and my_house_frozen_graph.pb.

If you want to downlad image pb file, you may change download-models.gradle file.

I think this is a good reference for anyone who want to know how tensorflow can be used by speech and android.

For more information, see Readme of each directory.

[You may click here to to git book for more material.](https://shichaog1.gitbooks.io/hand-book-of-speech-enhancement-and-recognition/content/)
可从淘宝、京东、当当购买本书。
《实时语音处理实践指南》，若如下链接失效，请在购买软件里搜索书名。
https://detail.tmall.com/item.htm?spm=a1z0d.6639537.1997196601.4.13f574848RXeNK&id=616382027158
