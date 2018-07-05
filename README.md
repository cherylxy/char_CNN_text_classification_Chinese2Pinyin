# char-CNN-text-classification-tensorflow

## [Here is an article explaining this code](http://blog.csdn.net/Irving_zhang/article/details/75634108) ##

## Reqirement ##
- Python 3.5.5
- Numpy 1.13.1
- TensorFlow 1.2.1-1.8

## Running ##
python training.py

## Models ##
charCNN.py : 9-layer large convolutional neural network based on raw character.

## Dataset ##
If dataset is not found under datasets_dir, it will be downloaded automatically. 
The feeding method is used now to get data into TF model.

-- ag: [AG](http://www.di.unipi.it/~gulli/AG_corpus_of_news_articles.html) is a collection of more than 1 million 
news articles. News articles have been gathered from more than 2000 news sources by ComeToMyHead in more than 1 year of 
activity. ComeToMyHead is an academic news search engine which has been running since July, 2004.


## ��ȷ����1e-4
������������epsilon=[0.01, 0.001, 1e-5]��ѧϰ��ΪĬ��0.001��
����ǣ�ǰ����̫�󣨣���ѧϰ����ʲôloss��1.3�𵴣�
1e-5�Ľ����Ĭ�ϵ�1e-8û����ͬ����step=4000���ұ��ˣ�Ȼ��������� ����ξ��飡
�ٱ��ظ�


##  ���ã�����лл���ķ��� Q: ����ѵ��3k�����ң�acc=0.8, loss=0.2���ң�ʱ��acc�轵����0.2��lossͻ������10000+����
Ȼ���������ص�0.7��acc�����ҡ��������г������������ԭ���������
PS: github���н���˵��Adam�����⣨https://stackoverflow.com/questions/42327543/adam-optimizer-goes-haywire-after-200k-batches-training-loss-grows/42420014#42420014����

���⣺restore��ʱ����˺ܴ�����