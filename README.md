# pytorch_multilabel_dataset
An implementation of a multilabel dataset for PyTorch. It builds from images plus xmls (or json) associated with each image.

XMLMultiLabelDataset class allows to build a PyTorch compatible dataset that has several labels per image. The labels are part of a 
hierarchy of classes (a class can be a child of another class). The labels are present on xml tags, it is expected to have a xml file
per image, thus, the image and xml share the same name besides the extension.

It is possible to get particular information from the hierarchy, such as indexes of children of a class, as well as names.
