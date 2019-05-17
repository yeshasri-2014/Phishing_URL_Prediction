# Phishing_URL_Prediction
Phishing URL prediction using ML Classification algorithms

A phishing website (sometimes called a "spoofed" site) tries to steal your account password or other confidential information by tricking you into believing you're on a legitimate website. You could even land on a phishing site by mistyping a URL (web address).

Inorder to avoid users accidentially share the sensitive information on malicious website, we need to detect those URL's.But there are 1000’s of phishing websites created daily, tracking them and avoiding users to access them is not possible.

We can visit the website’s like https://www.phishtank.com/ which track’s phishing websites to check whether the URL which we want to access is in the black list, but this require human intervention/manual effort

- Possible Solution:

To identify the phishing website’s we can use the machine learning algorithm’s so that we can automate the task of identify the phishing URL’s.Google and most of modern web browsers uses this sophisticated ML techniques to identify the phishing URL’s.

- As part of the dataset we have below columns, which are used to classify the URL as phishing or not

having_IP_Address { -1,1 }

URL_Length { 1,0,-1 }

Shortining_Service { 1,-1 }

having_At_Symbol { 1,-1 }

double_slash_redirecting { -1,1 }

Prefix_Suffix { -1,1 }

having_Sub_Domain { -1,0,1 }

SSLfinal_State { -1,1,0 }

Domain_registeration_length { -1,1 }

Favicon { 1,-1 }

port { 1,-1 }

HTTPS_token { -1,1 }

Request_URL { 1,-1 }

URL_of_Anchor { -1,0,1 }

Links_in_tags { 1,-1,0 }

SFH { -1,1,0 }

Submitting_to_email { -1,1 }

Abnormal_URL { -1,1 }

Redirect { 0,1 }

on_mouseover { 1,-1 }

RightClick { 1,-1 }

popUpWidnow { 1,-1 }

Iframe { 1,-1 }

age_of_domain { -1,1 }

DNSRecord { -1,1 }

web_traffic { -1,0,1 }

Page_Rank { -1,1 }

Google_Index { 1,-1 }

Links_pointing_to_page { 1,0,-1 }

Statistical_report { -1,1 }

Result { -1,1 }

- I have followed below procedure to predict the score.

. Dataset collection
. Pre profiling
. Cleaning the dataset
. Post profiling
. Analysis of Data to draw the insights
. Applied different ML classification algorithms. Calculated accuracy, precision,recall and F-score to choose the best model for prediction
. Deployed the model for prediction

- Conclusion

. Among all the classification algorithms tired,Random forest with the randomize search CV with best search parameters and Ensembling voting classifier are giving the best accuracy of 97%.

. One important item I want to highlight in this project is to test the actual phishing URL’s. Parsing URL into different columns fields was very interesting and challenging, truly admire how simple and efficient is python language.
