# GraphQL API Server CRUD using Express Tutorial

Youtube :
[https://youtu.be/Gg8ls8YcYq4](https://youtu.be/Gg8ls8YcYq4)

Queries :

```
mutation createPost(
  $input: PostInput
) {
  createPost(
    input: $input
  ) {
    id
    title
    content
  }
}
```
```
query getPosts {
  getPosts {
    id
    title
    content
  }
}
```
```
query getPost(
  $id: ID!
) {
  getPost(
    id: $id
  ) {
    id
    title
    content
  }
}
```
```
mutation updatePost(
  $id: ID!
  $input: PostInput
) {
  updatePost(
    id: $id
    input: $input
  ) {
    id
    title
    content
  }
}
```