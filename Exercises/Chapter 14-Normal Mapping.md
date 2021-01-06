## Chapter 14 | Exercises

#### 1.

#### (a) position, normal, texture coordinates, tangent-space basis

#### (b) blend weights, palette indices

#### 2.

```glsl
void main()
{
	vec3 worldPos = (worldMat * vec4(position, 1.0)).xyz;
    	vec3 Nor = normalize(transpose(inverse(mat3(worldMat)))*normal);
   	vec3 Tan = normalize(transpose(inverse(mat3(worldMat)))*tangent);
    	vec3 Bin = cross(Nor, Tan);
   	mat3 tbnMat = transpose(mat3(Tan,Bin,Nor));
    
    	v_lightTS = tbnMat*normalize(lightDir);
    	v_viewTS = tbnMat * normalize(eyePos - worldPos); 
    
    	v_texCoord = texCoord;
    	gl_Position = projMat * viewMat * vec4(worldPos, 1.0));
}
```

#### 3. 

$$
M_{TBN} ^ {-1}= \begin{pmatrix}
T_x & T_y & T_z \\\\
B_x & B_y & B_z \\\\
N_x & N_y & N_z 
\end{pmatrix} ^{-1}
$$



#### 4. In the context, we used to 2 neighbors to calculate tangent vector, which is the simplest method that has been introduced. Other method exists using more neighbor vectors to calculate tangent vectors.

#### 5.

```glsl
void main()
{
   vec3 normal = normalize(2.0 * texture(normalMap, v_texCoord).xyz - 1.0);
   vec3 light = normalize(v_lightTS);
  	
   vec3 matDiff = texture(colorMap, v_texCoord).rgb;
   vec3 diff = max(dot(normal,light),0.0) * srcDiff * matDiff;
  
   fragColor = vec4(diff, 1.0);
}
```



