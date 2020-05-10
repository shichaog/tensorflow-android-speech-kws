My book

![My book](https://github.com/shichaog/WebRTC-audio-processing/blob/master/book.png)

[天猫购买链接](https://detail.tmall.com/item.htm?spm=a220m.1000858.1000725.6.3a8e144cSO3Gp9&id=616382027158&areaId=330100&user_id=1932014659&cat_id=2&is_b=1&rn=919b763eb3051be569c91f85996e73eb)

[京东购买链接](https://item.jd.com/12838726.html)

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

