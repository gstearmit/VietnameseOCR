## Instructions

To get started, first clone this repo:

```
git clone  https://github.com/gstearmit/VietnameseOCR.git 
cd VietnameseOCR
```


Create and activate a conda env:
```
conda create -n vietnamese-ocr python=3.6.5
conda activate vietnamese-ocr
```

Or a venv (make sure your `python3` is 3.6+):
```
python3 -m venv venv
source venv/bin/activate  # for Windows, use venv\Scripts\activate.bat
```

Install all the requirements:

```
pip install -r requirements.txt
```

You can now run the app:
```
python train.py
```

and visit http://127.0.0.1:8050/.


Error "module 'tensorflow' has no attribute 'Session'"
TF1.x hello world:
```
    import tensorflow as tf
    msg = tf.constant('Hello, TensorFlow!')
    sess = tf.Session()
    print(sess.run(msg))
```
TF2.x hello world:
```
    import tensorflow as tf
    msg = tf.constant('Hello, TensorFlow!')
    tf.print(msg)
```

Kiểm tra cài đặt Với tensorflow GPU:
> python
>> import tensorflow as tf
>> sess = tf.Session(config=tf.ConfigProto(log_device_placement=True))