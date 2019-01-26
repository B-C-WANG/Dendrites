- use panel to get "load iris" of sklearn
![](/tutorial_iris/1.png)
- create a new pandas.DataFrame
![](/tutorial_iris/2.png)
- connection the output of iris data to input of DataFrame for creating a DataFrame of dataset
![](/tutorial_iris/3.png)
- use the button on the bottom to hide optional params
![](/tutorial_iris/4.png)
- use getattr to get feature of data
![](/tutorial_iris/5.png)
- getattr needs a string, use "New String"
![](/tutorial_iris/6.png)
- input "data", which same as XXX.data
![](/tutorial_iris/7.png)
- use key "ctrl" to copy the "getattr" block
![](/tutorial_iris/8.png)
- use key "W" to move the blackground left
![](/tutorial_iris/9.png)
- drag from DataFrame, then its instance method will show, type head to get DataFrame.head()
![](/tutorial_iris/10.png)
- get print block
![](/tutorial_iris/11.png)
- connect to the "return" of head, then run the program
![](/tutorial_iris/12.png)
- when a block is selected, its doc string will show 
![](/tutorial_iris/13.png)
- when a pin is dragged out, its doc string will show
![](/tutorial_iris/14.png)
- use a type convert block to convert DataFrame to numpy.ndarray
![](/tutorial_iris/15.png)
- convert to array
![](/tutorial_iris/16.png)
- print its shape, 150,4 which means n_sample is 150 and feature num is 4
![](/tutorial_iris/17.png)
- use the same way to get target, now we got both feature and target
![](/tutorial_iris/18.png)
- add a train test split block from sklearn
![](/tutorial_iris/19.png)
- we need args and kwargs, to create args, use "New Tuple", and click on left down button to add a custom "ANY" pin 
![](/tutorial_iris/20.png)
- the same way to create a "New **kwargs" block
![](/tutorial_iris/21.png)
- add new integer
![](/tutorial_iris/22.png)
- put our X (shape 150,4) and y (150,1) to tuple, and add some kwargs, e.g. we here use test_size=float(0.3), random_state=int(123)
![](/tutorial_iris/23.png)
- print out the result of train test split
![](/tutorial_iris/24.png)
- use slice to get the output of train test split
![](/tutorial_iris/25.png)
- the output of train test split is x_train,x_test,y_train and y_test
![](/tutorial_iris/26.png)
- create a New GradientBoostingClassifier from sklearn
![](/tutorial_iris/27.png)
- drag out the pin and find the "fit", then "predict"
![](/tutorial_iris/28.png)
- connect the X and y of "fit" to x_train and y_train, relatively, and connect x_test to X of "predict"
![](/tutorial_iris/30.png)
- run the program and the predict result is shown
![](/tutorial_iris/32.png)
- to make a judge, reshape y_test to (-1), keeps the same shape as y_pred
![](/tutorial_iris/33.png)
- do minus
![](/tutorial_iris/34.png)
- got the result, 0 means the right answer, -1 or 1 is wrong
![](/tutorial_iris/35.png)
- finally save our graph
![](/tutorial_iris/36.png)
- a total review
![](/tutorial_iris/37.png)