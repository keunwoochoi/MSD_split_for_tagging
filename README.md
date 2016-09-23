# MSD_split_for_tagging

By Keunwoo Choi

This split setting is used in [my ismir paper (Automatic Tagging using Deep Convolutional Neural Networks)](https://arxiv.org/abs/1606.00298) and [my icassp 2017 submission (Convolutional Recurrent Neural Networks for Music Classification)](https://arxiv.org/abs/1609.04243). 

As stated in the paper, I used [top 50 tags](https://github.com/keunwoochoi/MSD_split_for_tagging/blob/master/tags.py) except few too-obviously-not-related-to-audio-content ones. Also, I only count tag as valid if the ground truth > 50. (The value ranges in [0, 100]). + Of course only those with audio files were selected. (Very recently I found out there are some zero-sized files though.)

### x
There are three formats - 7d, MSD, and filename. One line, one value, i.e., separated by `\n`. No header. 

Filenames are in a format of `3/6/36122424.npy` for example. Probably you want to change it as `.clip.mp3` if you and I are connected by some colleagues :) 

### y
If you want to use the tags I selected, you can simply use the `{train, valid, test}_y.npy` as `y` labels. 

