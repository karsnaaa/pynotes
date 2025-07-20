---
title: Pandas
date: 2025-07-21
author: Your Name
cell_count: 23
score: 20
---

```python

```


```python
import pandas as pd  
from sklearn.model_selection import train_test_split
from sklearn.feature_extraction.text import CountVectorizer
from sklearn.naive_bayes import MultinomialNB
import streamlit as st
```


```python
data = pd.read_csv('C:/Users/HP/Desktop/OIB-SIP/emailspam/dataset-mail/spam.csv', encoding='latin-1')
```


```python
print("Original Shape:", data.shape)
```


```python
print(data.head())
```


```python
data = data[['v1', 'v2']]
```


```python
data.drop_duplicates(inplace=True)
```


```python
data.dropna(inplace=True)
```


```python
print("\nCleaned Shape:", data.shape)
```


```python
data['v1'] = data['v1'].replace(['ham', 'spam'], ['Not Spam', 'Spam'])
```


```python
data.rename(columns={'v1': 'Category', 'v2': 'Message'}, inplace=True)
```


```python
print("\nLabel Distribution:\n", data['Category'].value_counts())
```


```python
mess_train, mess_test, cat_train, cat_test = train_test_split(mess, cat, test_size=0.2, random_state=0, stratify=cat)
```


```python
cv = CountVectorizer(stop_words='english')
```


```python
features_train = cv.fit_transform(mess_train)
features_test = cv.transform(mess_test)
```


```python
model = MultinomialNB()
model.fit(features_train, cat_train)
```


```python
print("Accuracy:", model.score(features_test, cat_test))
```


```python
def predict(message):
  message = cv.transform([message]).toarray()
  result = model.predict(message)
  return result
```


```python
st.header("Email Spam Detector")
```


```python
output = predict("WINNER!! This is the secret code to unlock the money: C3421.")
print(output)
```


```python
input_message=st.text_input("Enter a message")
```


```python
if st.button('Go'):
    output=predict(input_message)
    st.text(output)
else:
    pass
```


```python

```


---
**Score: 20**