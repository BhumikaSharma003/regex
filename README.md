# regex
exercise question

# Python Regular Expression Exercise

This repository contains solutions to a Python regular expression exercise where three different regular expressions were implemented to address different cases. Below are the details of each case along with the provided solutions:

## Case 1: Extracting Twitter Handles

In this case, the objective was to extract all Twitter handles from a given text. The Twitter handle is defined as the text that appears after "https://twitter.com/" and consists of only alphanumeric characters (A-Z, a-z, 0-9), and underscores.

```python
import re

text = '''
Follow our leader Elon musk on twitter here: https://twitter.com/elonmusk, more information 
on Tesla's products can be found at https://www.tesla.com/. Also here are leading influencers 
for Tesla-related news,
https://twitter.com/teslarati
https://twitter.com/dummy_tesla
https://twitter.com/dummy_2_tesla
'''
pattern = 'https:\/\/twitter.com\/[a-zA-Z_0-9]+'
print("Twitter Handles:")
print(re.findall(pattern, text))
