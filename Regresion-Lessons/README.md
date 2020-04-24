# Regression Lessons Resume (Supervised Machine Learning)
## Absolute Trick
![\Huge y = (w_1 + p \alpha) x + (w_2 + \alpha)](https://render.githubusercontent.com/render/math?math=%5CLarge%20y%20%3D%20(w_1%20%2B%20p%20%5Calpha)%20x%20%2B%20(w_2%20%2B%20%5Calpha))

Where:
* ![w_1](https://render.githubusercontent.com/render/math?math=w_1) : slope in the equation
* ![w_2](https://render.githubusercontent.com/render/math?math=w_2) : intercept in y axis
* ![p](https://render.githubusercontent.com/render/math?math=p) : coordinate in ![(p,q)](https://render.githubusercontent.com/render/math?math=(p%2Cq))
* ![\alpha](https://render.githubusercontent.com/render/math?math=%5Calpha) : Learning ratio

## Square Trick
![\Large y=(w_1+p(q-q')\alpha)x+(w_2+(q-q')\alpha)](https://render.githubusercontent.com/render/math?math=%5CLarge%20y%3D(w_1%2Bp(q-q')%5Calpha)x%2B(w_2%2B(q-q')%5Calpha))

Where:
* ![w_1](https://render.githubusercontent.com/render/math?math=w_1) : slope in the equation
* ![w_2](https://render.githubusercontent.com/render/math?math=w_2) : intercept in y axis
* ![p](https://render.githubusercontent.com/render/math?math=p) : coordinate in ![(p,q)](https://render.githubusercontent.com/render/math?math=(p%2Cq))
* ![q](https://render.githubusercontent.com/render/math?math=q) : coordinate in ![(p,q)](https://render.githubusercontent.com/render/math?math=(p%2Cq))
* ![q'](https://render.githubusercontent.com/render/math?math=q') : result of the evaluation of ![(p,q)](https://render.githubusercontent.com/render/math?math=p) in the original equation
* ![\alpha](https://render.githubusercontent.com/render/math?math=%5Calpha) : Learning ratio
 
## Mean Absolute Error
![\Large Error=\frac{1}{m} \sum_{i=1}^m  |y-\hat{y}|](https://render.githubusercontent.com/render/math?math=%5CLarge%20Error%3D%5Cfrac%7B1%7D%7Bm%7D%20%5Csum_%7Bi%3D1%7D%5Em%20%20%7Cy-%5Chat%7By%7D%7C)

Where:
* ![m](https://render.githubusercontent.com/render/math?math=m) : Number of points in the dataset
* ![y](https://render.githubusercontent.com/render/math?math=y) : Coordinate in point ![(x,y)](https://render.githubusercontent.com/render/math?math=(x%2Cy))
* ![\hat{y}](https://render.githubusercontent.com/render/math?math=%5Chat%7By%7D) : Predicted coordinate by function

## Mean Squared Error
![\Large Error=\frac{1}{2m} \sum_{i=1}^m  (y-\hat{y})^2](https://render.githubusercontent.com/render/math?math=%5CLarge%20Error%3D%5Cfrac%7B1%7D%7B2m%7D%20%5Csum_%7Bi%3D1%7D%5Em%20%20(y-%5Chat%7By%7D)%5E2)
* ![m](https://render.githubusercontent.com/render/math?math=m) : Number of points in the dataset
* ![y](https://render.githubusercontent.com/render/math?math=y) : Coordinate in point ![(x,y)](https://render.githubusercontent.com/render/math?math=(x%2Cy))
* ![\hat{y}](https://render.githubusercontent.com/render/math?math=%5Chat%7By%7D) : Predicted coordinate by function

## Gradient Descent
![\Large w_i \rightarrow w_i - \alpha \frac{\partial}{\partial w_i}Error](https://render.githubusercontent.com/render/math?math=%5CLarge%20w_i%20%5Crightarrow%20w_i%20-%20%5Calpha%20%5Cfrac%7B%5Cpartial%7D%7B%5Cpartial%20w_i%7DError)

Where:
* ![w_i](https://render.githubusercontent.com/render/math?math=w_i) : next estimated point / last estimated point
* ![\alpha](https://render.githubusercontent.com/render/math?math=%5Calpha) : learning rate
* ![Error](https://render.githubusercontent.com/render/math?math=Error) : Error function to minimize