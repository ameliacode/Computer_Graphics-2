## Chapter 13 | Exercises

#### 1. 

#### (a) It transforms spine's vertex to the bone space of its parent, pelvis

#### (b) It transforms bone space into spine's character space

#### (c) 

$$
M_{5,d}M_{6,p}
$$

#### (d) 

Top to down, 
$$
M_{1,d}^{-1} = I
$$
$$
M_{4,p}^{-1}, M_{4,d}^{-1} = M_{4,p}^{-1}M_{3,d}^{-1}
$$

#### 2.

#### (a)

$$
M_{f,p} = \begin{pmatrix}
1 & 0 & 12 \\\\
0 & 1 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
,M_{h,p} = \begin{pmatrix}
1 & 0 & 10 \\\\
0 & 1 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (b)

$$
M_{f,d} = M_{u,d}M_{f,p} = \begin{pmatrix}
1 & 0 & 12 \\\\
0 & 1 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
,M_{h,d} = M_{f,d}M_{h,p} = \begin{pmatrix}
1 & 0 & 22 \\\\
0 & 1 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (c)

$$
M_{f,d}^{-1} = \begin{pmatrix}
1 & 0 & -12 \\\\
0 & 1 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
,M_{h,d}^{-1} = \begin{pmatrix}
1 & 0 & -22 \\\\
0 & 1 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (d)

$$
M_{f,l} = \begin{pmatrix}
0 & -1 & 0 \\\\
1 & 0 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
,M_{h,l} = \begin{pmatrix}
0 & 1 & 0 \\\\
-1 & 0 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (e)

$$
M_{f,a} = M_{u,a}M_{f,p}M_{f,l}=\begin{pmatrix}
0 & -1 & 12 \\\\
1 & 0 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (f) 

$$
M_{h,a} = M_{f,a}M_{h,p}M_{h,l}=\begin{pmatrix}
1 & 0 & 12 \\\\
0 & 1 & 10 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (g)

$$
w_fM_{f,a}v_f + w_hM_{h,a}v_h = (11,9)
$$

#### 3.

#### (a) Same as 2 - (a)

#### (b) Same as 2 - (b)

#### (c) Same as 2 - (c)

#### (d) 

$$
M_{f,l} = \begin{pmatrix}
0 & 1 & 0 \\\\
-1 & 0 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
,M_{h,l} = \begin{pmatrix}
0 & -1 & 0 \\\\
1 & 0 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (e)

$$
M_{f,a} = M_{u,a}M_{f,p}M_{f,l}=\begin{pmatrix}
0 & 1 & 12 \\\\
-1 & 0 & 0 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (f)

$$
M_{h,a} = M_{f,a}M_{h,p}M_{h,l}=\begin{pmatrix}
1 & 0 & 12 \\\\
0 & 1 & -10 \\\\
0 & 0 & 1
\end{pmatrix}
$$

#### (g)

$$
w_fM_{f,a}v_f + w_hM_{h,a}v_h = (11,-9)
$$

#### 4.

#### (a) (2,0)

#### (b) 

$$
M_{f,p}M_{f,l}
$$

#### (c) (-1,0)

#### (d)

$$
M_{f,p}M_{f,l}M_{h,p}M_{h,l}
$$
#### (e) (3.8,-2.2)

$$
M_{f,a} = M_{u,a}M_{f,p}M_{f,l}=\begin{pmatrix}
0 & 1 & 4 \\\\
-1 & 0 & 0 \\\\
0 & 0 & 1
\end{pmatrix},M_{h,a} = \begin{pmatrix}
1 & 0 & 4 \\\\
0 & 1 & -3 \\\\
0 & 0 & 1
\end{pmatrix} 
$$
$$
v_f = M_{f,d}^{-1}v, v_h = M_{h,d}^{-1}v
$$
$$
w_fM_{f,a}v_f + w_hM_{h,a}v_h = (3.8,-2.2)
$$
#### 5.

#### (a) quaternions and translational vectors 

Two data are interpolated independently in each bone space per frame.

#### (b) positions, normals, texture coordinates, palette indices, blend weights 

#### 6.

#### (a) 12 bones

#### (b) 3 vertices

#### (c) 0.6

#### (d) 

Md remains fixed throughout the entire animation which transforms character space into bone space, whereas Ma is updated for every frame.
$$
M_i = M_{i,a}M_{i,d}^{-1}
$$
#### 7.  IK is applied to the head bone. 

