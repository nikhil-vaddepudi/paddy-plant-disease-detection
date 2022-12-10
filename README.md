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

## Image Segmentation
It employs to reduce image’s complexity and simplify it.

A K-means clustering technique has been engaged in this. K means clustering partitions or makes the clusters of the data which is nearest to the centroid. Centroid is arithmetic mean of the all cluster points. The new centroid is estimated for each of the partition or cluster, after allocating the nearest centroid. The position and number of the centroid is changed step by step till k-clusters are derived and no more changes are possible.

The crucial part of this technique is selecting the K values. The values will be taken by using trial and error method.

## Classification of Images

We didi it by using CNN, VGG-19, Inception v3 and compared with each other

