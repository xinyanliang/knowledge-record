# Medical ![Maintenance](https://img.shields.io/maintenance/yes/2017.svg) [![DUB](https://img.shields.io/dub/l/vibe-d.svg)](LICENSE)
## [Home](../../README.md)
- The goal of this document is to provide a reading list in Medical.


## Topics
- [The type of the edical images](#the-type-of-the-medical-images)
- [Pipeline for the medical tasks](#pipeline-for-the-medical-tasks)
- [Disease](#disease)
- [Papers](#papers)
- [Lab](#lab)
- [People](#people)
- [Datasets](#datasets)
- [Software](#software)
- [References](#references) 

## Disease
 [Alzheimer’s disease](https://en.wikipedia.org/wiki/Alzheimer%27s_disease) (AD) and its prodrome, mild cognitive impairment (MCI).

[Topics](#topics)

## The type of the medical images
[MRI](https://en.wikipedia.org/wiki/Magnetic_resonance_imaging)(Magnetic resonance imaging)
is a medical imaging technique used in radiology to form pictures of the anatomy and the physiological processes of the body in both health and disease. MRI scanners use strong magnetic fields, radio waves, and field gradients to generate images of the organs in the body. MRI does not involve x-rays, which distinguishes it from computed tomography (CT or CAT).

[PET](https://en.wikipedia.org/wiki/Positron_emission_tomography)(Positron emission tomography)
is a nuclear medicine functional imaging technique that is used to observe metabolic processes in the body. The system detects pairs of gamma rays emitted indirectly by a positron-emitting radionuclide (tracer), which is introduced into the body on a biologically active molecule. Three-dimensional images of tracer concentration within the body are then constructed by computer analysis. In modern PET-CT scanners, three-dimensional imaging is often accomplished with the aid of a CT X-ray scan performed on the patient during the same session, in the same machine.

[Positron emission tomography–computed tomography](https://en.wikipedia.org/wiki/PET-CT) (better known as PET-CT or PET/CT) is a nuclear medicine technique which combines, in a single gantry, a positron emission tomography (PET) scanner and an x-ray computed tomography (CT) scanner, to acquire sequential images from both devices in the same session, which are combined into a single superposed (co-registered) image. Thus, functional imaging obtained by PET, which depicts the spatial distribution of metabolic or biochemical activity in the body can be more precisely aligned or correlated with anatomic imaging obtained by CT scanning. Two- and three-dimensional image reconstruction may be rendered as a function of a common software and control system.

## 图片格式

- [NlfTl-1](https://nifti.nimh.nih.gov/nifti-1/)

- [NlfTl-2](https://nifti.nimh.nih.gov/nifti-2/)

- [DICOM](http://www.dicomstandard.org/)

- [NACC数据类型介绍](https://www.alz.washington.edu/WEB/forms_bioimag.html)

## Pipeline for the medical tasks

[常见医疗扫描图像处理步骤](http://shartoo.github.io/medical_image_process/)
<ol>
<li>Image preprocessing and feature extraction
	<ol>
		<li>skull-stripped </li>
		<li>cerebellum-removed</li>
	</ol>
</li>
</ol>


[Topics](#topics)

## Papers
Paper list.

|No.  |Figure   |Title   |Authors  |Pub.  |Links|Datasets|
|-----|:-----:|:-----:|:-----:|:-----:|:---:|:---:|
|1|![Smile](paper_image/shiyinghuang2014cvpr.png)|__Joint Coupled-FeatureRepresentation and Coupled Boosting for AD Diagnosis__|[Yinghuan Shi](https://cs.nju.edu.cn/shiyh/), [Heung-Il Suk](https://www.ku-milab.org/people), Yang Gao, [Dinggang Shen](https://www.unc.edu/~dgshen/) |__[CVPR 2014](http://www.cvpapers.com/cvpr2014.html)__|[PDF](pdf/Joint Coupled-FeatureRepresentation and Coupled Boosting for AD Diagnosis.pdf) <br/> | ADNI|

### 2016
|No|Titel|Links|
|---|:---|:---|
|1.|Alzheimer's disase diagnostics by as deeply supervised adaptable 3D convolutional network.pdf|[paper](https://arxiv.org/pdf/1607.00556.pdf)|

### 2014
|No|Titel|Links|
|---|:---|:---|
|1|__Joint Coupled-FeatureRepresentation and Coupled Boosting for AD Diagnosis__|[paper](pdf/Joint Coupled-FeatureRepresentation and Coupled Boosting for AD Diagnosis.pdf)|

[Topics](#topics)

## Lab

|Name|主任|介绍|
|---|---|---|
|[LONI](http://loni.usc.edu/)| |(Laboratory of Neuro Imaging) is in Keck School of Medicine of USC[University of Southern California](https://www.usc.edu/).|
|[MiLab](https://www.ku-milab.org/)| |(Machine Intelligence Laboratory at [Korea University](https://www.korea.edu/)) is devoted to the development of computational models and their applications to various researches in the brain and cognitive engineering field. Specifically, we focus on 1) pattern recognition and machine learning algorithms inspired from the neural information processing mechanism in a human brain, 2) brain disease diagnosis or prognosis by analyzing complex patterns inherent in neuroimaging or genetic data, and 3) non-invasive brain-computer interfaces to enhance human performance.
|[IDEA Lab](http://www.med.unc.edu/bric/ideagroup/core-labs/idea-research-lab)| | |
|[ibrain](http://ibrain.nuaa.edu.cn/)| 张道强| |

[Topics](#topics)

## People
|Name|研究方向|
|---|---|
|[刘勇](http://www.cebs.ac.cn/duiwu_teacher.php?id=88) ||
|[隋婧](http://www.cebs.ac.cn/duiwu_teacher.php?id=66)||
|[duliang](https://github.com/liangdu/Deep-Learning-for-Medical-Applications)||

[Topics](#topics)

## Datasets

|Name|介绍|
|---|---|
|[ADNI]((http://adni.loni.usc.edu/))| [介绍](http://blog.csdn.net/sungden/article/details/79007264)


[数据集总结](http://blog.51cto.com/apinetree/1566203)

[Topics](#topics)

## Software
[LONI](http://loni.usc.edu/Software/)

查看CT扫描文件软件 [Mango](http://ric.uthscsa.edu/mango/)

读取dcm文件 [pydicom](http://pydicom.readthedocs.io/en/stable/getting_started.html). 参考Kaggle [Data Science Bowl 2017](https://www.kaggle.com/c/data-science-bowl-2017/data)

读取mhd格式 [SimpleITK](http://www.simpleitk.org/)

[大量的python库](http://www.nipy.org)

[simpleITK](http://insightsoftwareconsortium.github.io/SimpleITK-Notebooks/)


[MIPVA](https://mipav.cit.nih.gov/clickwrap.php)

[FSL](https://fsl.fmrib.ox.ac.uk/fsl/fslwiki/) 将MR脑图分割出灰质(GM)、白质(WM)和脑脊液(CSF)

[RAVENS](http://iatr.virtualbrain.org/tool_review.php?tool_id=86)  Regional volumetric analysis of brain images

[Nipype](http://nipype.readthedocs.io/en/latest/)

[Topics](#topics)

## References
[医学影像学习](http://www.yxppt.com/)

[matlab处理dicom](http://blog.csdn.net/ymqq1/article/details/8765742)

[paper](https://wizardyan.github.io/2017/08/29/paper_notes_6/)

[Topics](#topics)



## others

