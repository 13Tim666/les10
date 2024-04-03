import pandas as pd
import random
lst = ['robot','robot','human','human','robot']
data = pd.DataFrame({'whoAmI':lst})
data['index'] = data.reset_index().index
one_hot = data.pivot(index='index', columns='whoAmI', values='whoAmI').notnull().astype(int)
one_hot.reset_index(drop=True, inplace=True)
one_hot.head()
