<h1 style="margin: auto; width: 100%; text-align: center; font-size: 25px;">Music Genre Classification</h1>

<h3>This program identifies classical, jazz, rock, and hip hop music. Will implement multi-label functionality soon.</h3>
 
Packages required: pytube, moviepy, pydub, fastai, fastaudio (install with pip)

Implements my dataset on <a href="https://www.kaggle.com/datasets/benfitzgerald3132/jazz-vs-classical-music-classification/">Kaggle</a> and <a href="https://github.com/bfitzgerald3132/jazz-classical-dataset">GitHub</a>

Attained 90.77% accuracy with batch_size = 64, epoch_count = 6, learning_rate = 4e-2

<img src="https://github.com/bfitzgerald3132/MusicGenreClassification/blob/main/updated_screenshot.png" />

File breakdown: <ul>
<li>"Train Classifier.ipynb": Code used to train model</li>
<li>"Classify Audio.ipynb": Notebook where users can test a clip's genre</li>
<li>"multi_category_classifier.pkl": Pkl-ed model parameters</li> </ul>
------------------------------

<h2>Installation and execution:</h2>

Download the attached ZIP file, extract, and run in Jupyter Notebook. Dependencies updated/installed automatically.
