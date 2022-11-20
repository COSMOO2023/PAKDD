# PAKDD 2023

We use two real-world datasets, TaxiBJ and TaxiNYC, in our comparisons. The details of TaxiBJ dataset are demonstrated in the paper, and we further show the descriptions and performance of TaxiNYC dataset in the following paragraphs.

The public TaxiNYC dataset [20] consists of the taxi demand and the time meta. The taxi demand covers the shared taxi pick-up and drop-off data in New York from July 2015 to December 2015. In TaxiNYC dataset, we follow the principle of Wang et al. [21]. We keep the last 10% data as the testing set and the rest as the training set. The time interval is $30$ minutes, and the entire city is divided into a $32\times32$ grid map in both datasets. The demand values of both datasets are scaled into $[-1,1]$ by Min-Max Normalization. In the evaluation, we re-scale the predicted value back to the normal values, compared with the ground truth. In the evaluation, we re-scale the predicted value back to the normal values, compared with the ground truth.

Similar to Table 1, we show experimental results of our proposed method in Table 3, which are COSMOO-b and COSMOO-a. As shown in Table 3, we observe that LPB shows a very good earliness with worst prediction accuracy performances because it does not consider a continuous updating mechanism. However, the UFI (1 hr) performs the best accuracy result but has unfavorable earliness and updating frequency performances. Compared with the other competing methods, COSMOO methods, including COSMOO-a and COSMOO-b, demonstrate superiority in prediction accuracy, earliness, and frequency. 
Different from the first experiment, the COSMOO-a and COSMOO-b show the same performance in the TaxiNYC dataset. The reason is that the TaxiNYC dataset does not contain any unexpected deviation situations. Hence the advanced PBCU strategy is reduced to the basic PBCU strategy.


![TaxiNYC](https://user-images.githubusercontent.com/118663456/202898408-9de180da-2dc1-4233-b1e9-e09effa21f4e.jpg)


[20] NYC Taxi and Limousine Commission (TLC): Tlc trip record data. https://www1.nyc.gov/site/tlc/about/tlc-trip-record-data.page (2015)

[21] Wang, Y., Yin, H., Chen, H., Wo, T., Xu, J., Zheng, K.: Origin-destination matrix prediction via graph convolution: a new perspective of passenger demand modeling. In: Proceedings of the 25th ACM SIGKDD international conference on knowledge discovery & data mining. pp. 1227–1235 (2019)
