# Heyo 
## The FineVideo Dataset
The description is largely just copy-pasted from some notes I was taking as I was doing the assignment apologies for the repeition. 

But TLDR I came across this dataset while scrubbing huggingface and it seemed interesting. 

It contains 43,751 creative commons licensed yt videos and each video was annotated by first gemini 1.5 pro and the cleaned up by gpt-4o it was an attempt to open-source a large dataset for VLM finetuning and training and it was espceially interesting to me because most often these types of large expensive to gather datasets are only owned by big companies. 

I only downloaded the metadata aspects of this dataset and none of the almost 700gbs of videos that came with it. 

for the dataset viz and the assignment you will see that there are 2 csv's 

one is the original videos.csv
with is 43751 rows x 19 cols
for each video it contained all the original metadata associated with that video. Things such as view counts, likes, comments, upload date etc etc, all of these are interseting but for simplicity and this assignment I focused on duration + transcript 

These videos were also split into AI derived and generated categories 

The 2nd csv I need to disclaim I had claude help parse through the videos.csv above and chunk the transcript itself into percentage based chunks. I didn't have enough time to figure out how to setup a mapped time-code -> transcript dataset into a csv...so this 2nd csv I used in the assignment is a extration of the overall transcript/videos dataset. It is 10% of the overall dataset with the transcript chunked into 10% chunks, this way it would be easier for me to process and find out about how people tend to organize and structure their videos. In the future would love to figure out that mapping thing....

But either way, this transcript_tenths csv contains a smaller slice of the original videos.csv dataset

containing the same video ID and associated metadata that way it would be simple to merge/group them together later.


