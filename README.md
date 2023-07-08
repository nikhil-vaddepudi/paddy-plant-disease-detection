# paddy-plant-disease-detection using deep learning

## Image Acquisition :-
A total of 10407 training images and 3469 testing images were collected from different agricultural websites and paddy fields.   These images are captured in 480×640 pixels. </br>
These are from the Kaggle  link:https://www.kaggle.com/competitions/paddy-disease-classification/data


<table class='center'>
  <tr>
    <th>Class Name </th>
    <th>No of Images</th>
  </tr>
  <tr>
    <td>Bacterial Leaf Blight</td>
    <td>479</td>
  </tr>
  <tr>
    <td>Bacterial leaf streak</td>
    <td>380</td>
  </tr>
  <tr>
    <td>Bacterial panicle blight</td>
    <td>337</td>
  </tr>
  <tr>
    <td>Blast</td>
    <td>1738</td>
  </tr>
  <tr>
    <td>Brown spot</td>
    <td>965</td>
  </tr>
  <tr>
    <td>Dead heart</td>
    <td>1442</td>
  </tr>
  <tr>
    <td>Downy mildew</td>
    <td>620</td>
  </tr>
  <tr>
    <td>Hispa</td>
    <td>1594</td>
  </tr>
  <tr>
    <td>tungro</td>
    <td>1088</td>
  </tr>
  <tr>
    <td>Normal</td>
    <td>1764</td>
  </tr>
</table>


## Image Pre-processing 
### Image resizing
In pre-processing, the image size is increased. The reason is that reducing the size of the image removes high-frequency information. The more of it size remove, the less specific the representation becomes. Everyone would expect that decreasing image size would decrease false negatives and increase false positives, but again, that depends on what kind of categories that are trying to classify. For any particular problem, there is probably a “sweet spot”, an image size that yields the maximum accuracy. For the data set that we considered, the image was resized to 640 x 480 from 480 x 480.

### Splitting dataset
 To train a deep learning model. We need to have a training set and a validation set. For verification, we need to have a testing set too.
 The data set,consisting of 10407 images, is divided into three categories:
<ul>
  <li> Training set with 7280 images (70%). </li>
  <li> Validation set with 1036 images (10%).</li>
  <li> Testing set with 2091 images (20%).</li>
</ul>

## Classification of Images

We used 6 pretrained models with additional layers (transfer learning) and compared the results between them.
The pretrained models that used are:
<ol>
  <li> ResNet101 v2</li>
  <li> Inception v3</li>
  <li> Inception - ResNet v2</li>
  <li> DenseNet201 </li>
  <li> MobileNet v2</li>
  <li> Xception </li>
  </ol>

