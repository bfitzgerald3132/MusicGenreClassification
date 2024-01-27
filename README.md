<h1 style="margin: auto; width: 100%; text-align: center; font-size: 25px;">Music Genre Classification</h1>

<h3>This program identifies classical, jazz, rock, and hip hop music. Will implement multi-label functionality soon.</h3>
 
Packages required: pytube, moviepy, pydub, fastai, fastaudio (install with pip)

Implements my dataset on <a href="https://www.kaggle.com/datasets/benfitzgerald3132/jazz-vs-classical-music-classification/">Kaggle</a> and <a href="https://github.com/bfitzgerald3132/jazz-classical-dataset">GitHub</a>

<h2>Accuracy:</h2>

My model attained 90.77% unadjusted accuracy classifying a 5-second WAV file with batch_size = 64, epoch_count = 6, learning_rate = 4e-2.

Adjusted accuracy is calculated by splitting an audio file into 5-second WAV segments and finding the most commonly predicted label. If a model correctly classifies a classical music clip 90.77% of the time, we can estimate that it classifies a clip as jazz, rock, or hip hop about 3.07% of the time. Therefore, an classical clip C split into _n_ 5-second segments must classify at least n/4 segments as the same incorrect genre to make an incorrect prediction. 

The model's adjusted inaccuracy is this given by Ia = (3.07/100) ^ n/4, for all n > 4. For a three-minute piece of classical music, this translates to an adjusted inaccuracy of Ia = 1.9683E-14. Adjusted accuracy therefore approaches 100% as n --> &infin;.

<img src="https://github.com/bfitzgerald3132/MusicGenreClassification/blob/main/updated_screenshot.png" />

File breakdown: 
<ul>
<li>"Train Classifier.ipynb": Code used to train model</li>
<li>"Classify Audio.ipynb": Notebook where users can test a clip's genre</li>
<li>"multi_category_classifier.pkl": Pkl-ed model parameters</li></ul>
------------------------------

<h2>Installation and execution:</h2>

Download the attached ZIP file, extract, and run in Jupyter Notebook. Dependencies updated/installed automatically.
