## Chapter 10 | Exercises

<<<<<<< HEAD
#### 1.

#### 2.

#### 3.

#### 4.

#### 5.

#### 6.

=======
#### 1. 2

5 cases of updating z buffer on a single fragment color:

* 0 (no triangle exists on a pixel) and 1, 2, 3, 4

Answer: 10(total times) / 5 (cases) = 2

#### 2. (0.5,0.25,0.25)

#### 3. (0.25,0.25,0.5)

#### 4. (a) f5, f3, f4, f2, f1 or f3, f5, f4, f2, f1 in order

Not all alpha values are 1 in five fragments, Hence, they must be processed in a back-to-front order after all opaque primitives are processed. 

#### (b)  (0.5,0.25,0.5)

#### 5.

From the question, the fog factor increases as the distance from the viewer increases. Hence, 
$$
f = \frac{ViewpointDistance - F}{F-N}
$$


#### 6.

If all three triangles' opacity value is 0.5 respectively, there would be no problem for this.

However, if all three have different values, sorting triangle cannot solve this matter. 

#### (a) the lower right part should be depicted "more blue-ish"

#### (b) 

Problem encountered: can't overwrite(blue polygon) an already rendered triangle(red one).

This can't be solved by sorting, only by splitting at least one triangle into several smaller triangles can resolve this.

Reference: 

[triangles colors render on top of each other]: https://answers.unity.com/questions/1373605/triangles-colors-render-on-top-of-each-other.html



>>>>>>> eb500b1fd7ec17dedd67ad117607549d93d84df1
