# Iris-Classification
This is the first Supervised Learning project that I have done! :) 

Here, I first visualied the dirstribution of the Iris dataset. And the most interesting outcome is that we can classify one class based on just one feature `Petal Length`.

![image](https://github.com/mahdis-repo/Iris-Classification/assets/145799768/d5bb4fff-4cb1-4e9c-90dd-3f0aa6daf475)

## dividing the dataset into train and test
I devided the dataset experiment a little on the learning process of the models:

```
from sklearn.model_selection import train_test_split

X = iris.drop(columns = ['Species'])
Y = iris['Species']
# train 60
# test 40
X_train0, X_test0, y_train0,  y_test0 = train_test_split(X, Y, test_size = 0.4, random_state = 0)
# train 70
# test 30
X_train1, X_test1, y_train1,  y_test1 = train_test_split(X, Y, test_size = 0.3, random_state = 0)
# train 80
# test 20
X_train2, X_test2, y_train2,  y_test2 = train_test_split(X, Y, test_size = 0.2, random_state = 0)
# train 90
# test 10
X_train3, X_test3, y_train3,  y_test3 = train_test_split(X, Y, test_size = 0.1, random_state = 0)
```

## models:
I implemented 9 different models with both tensorflow and sci-kit learn to see which ratio of test to train worked best with respect to the complexity of the models.

## Note:
This is a fairly small dataset, so maybe I try this experimental process later on a larger dataset.
