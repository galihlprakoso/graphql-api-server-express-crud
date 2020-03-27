queries :

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

query getPosts {
  getPosts {
    id
    title
    content
  }
}

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