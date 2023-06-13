This program was created to process COCO dataset for purpose of using it with YOLOv5 model.
We have selected 19 classes that we want the dataset to contain and discard other classes.
This program will read the label files, remove lines which class is not one of the 19 classes and then
reindex the classes so that class indexes are from 0 to 19.

how to use it?

first run: ./create_input_output_dirs.sh

then copy label files into input/labels/

to run the program:

iex -S mix

and then in iex shell:

ReindexLabels.main

You will find result in the output directory
