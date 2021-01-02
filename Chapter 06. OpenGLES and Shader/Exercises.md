## Exercises

#### 1.

```
void main(){
    gl_Position = projMat * viewMat * worldMat * vec4(position, 1.0);
    v_normal = normalize(transpose(inverse(mat3(worldMat))) * normal);
    v_texCoord = texCoord;
}
```

```c++
glEnableVertexAttribArray(0); // position
glVertexAttribPointer(0, 3, GL_FLOAT, GL_FALSE,
                     sizeof(Vertex), (const GLvoid*) offsetof(Vertex, pos));

glEnableVertexAttribArray(1); // normal
glVertexAttribPointer(1, 3, GL_FLOAT, GL_FALSE,
                     sizeof(Vertex), (const GLvoid*) offsetof(Vertex, nor));

glEnableVertexAttribArray(2); //texture coordinates
glVertexAttribPointer(2, 2, GL_FLOAT, GL_FALSE,
                     sizeof(Vertex), (const GLvoid*) offsetof(Vertex, tex));

```

#### 2. 

#### (a)

indexed representation:

```c++
glDrawElements(GL_TRIANGLES, 24, GL_UNSIGNED_SHORT, 0);
```

24 = 8(triangles) * 3(for each index array)

#### (b)

non-indexed representation:

```
glDrawArrays(GL_TRIANGLES, 0, 24);
```

