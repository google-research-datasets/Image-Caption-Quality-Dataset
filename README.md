# Image Caption Quality Dataset

A dataset of crowdsourced ratings for machine-generated image captions.

## Motivation

Image Captioning models can automatically generate natural language descriptions for input images.
To assess the quality of these model, researchers conduct human evaluations where raters are asked to judge the quality of model-generated captions for previously unseen images.

In this dataset, we provide a compilation of human ratings obtained for thousands of images and corresponding machine-generated captions that we have collected over the years from our evaluations.
See [Google Crowdsource](https://crowdsource.google.com/new-contribute/image-captioning/en) for our evaluation setup.

#### Sample application: Quality Estimation
Though human evaluation setup works well during development, it cannot be used to assess the quality of a caption in realtime when a model is deployed to serve live production traffic.
This dataset can be used to build an automatic Quality Evaluation (QE) model for Image Captioning to estimate the quality.


## Downloads

The dataset can be downloaded as a zip of tab-separated-values (TSV) files for train/dev/test split and corresponding image metadata.
Images have been sampled from the [Open Images Dataset](https://storage.googleapis.com/openimages/web/index.html).
Please see the metadata files or the Open Images website to download the image files.

### v1.0

Released: August 2019

[Download](https://storage.cloud.google.com/gcc-data/OID-rated-image-caption/v1/oid.rated-image-captions.v1.zip?organizationId=433637338589)

<table>
  <tr>
    <td><b>Fold</b></td>
    <td><b>Samples</b></td>
    <td><b>Unique Images</b></td>
  </tr>
  <tr>
    <td>Train</td>
    <td>58,354</td>
    <td>11,027</td>
  </tr>
  <tr>
    <td>Dev</td>
    <td>2,392</td>
    <td>6,54</td>
  </tr>
  <tr>
    <td>Test</td>
    <td>4,592</td>
    <td>1,237</td>
  </tr>
</table>


### v2.0

Released: September 2019

[Download](https://storage.cloud.google.com/gcc-data/OID-rated-image-caption/v2/oid.rated-image-captions.v2.zip?organizationId=433637338589)


<table>
  <tr>
    <td><b>Fold</b></td>
    <td><b>Samples</b></td>
    <td><b>Unique Images</b></td>
  </tr>
  <tr>
    <td>Train</td>
    <td>129,759</td>
    <td>28,525</td>
  </tr>
  <tr>
    <td>Dev</td>
    <td>7,151</td>
    <td>3,444</td>
  </tr>
  <tr>
    <td>Test</td>
    <td>7,135</td>
    <td>3,442</td>
  </tr>
</table>



### T2 Test Set

Released: June 2019

[Download](https://storage.cloud.google.com/gcc-data/cvpr2019/cvpr2019.cc-workshop.zip?organizationId=433637338589&_ga=2.185119273.-1459768570.1557891230)

During the [Conceptual Captions Challenge Workshop](http://www.conceptualcaptions.com) at CVPR 2019, we released a human ratings dataset for image captions called the [T2 Dataset](http://www.conceptualcaptions.com/challenge).
This dataset has ratings for the top 5 models in the challenge ([Leaderboard](http://www.conceptualcaptions.com/winners-and-data)).
The images in this set are disjoint from the images in all other versions above, and our recommendation is to use this as a test set for all versions of the Image Caption Quality Dataset.


## Dataset Description

See the README.txt file in the downloaded zip file for the version.


## Citation

If you use this dataset in your research, please cite our paper:

```
@article{icqd2019,
  title={Quality Estimation for Image Captions Based on Large-scale Human Evaluations},
  author={T. Levinboim, A. Thapliyal, P. Sharma, and R. Soricut},
  journal={arXiv preprint arXiv:1909.03396},
  year={2019}
}
```

## Contact us

If you have a technical question regarding the dataset or publication, please create an issue in this repository.
This is the fastest way to reach us.

If you would like to share feedback or report concerns regarding the data, please see OWNERS file for our contact information.
