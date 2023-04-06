# GraphQL

## Query

```graphql
query {
  fieldName(arg: "value") {
    subField
    anotherSubField
  }
}
```

## Mutation

```graphql
mutation {
  mutationName(input: { field: "value" }) {
    field
  }
}
```

## Fragment

```graphql
fragment MyFragment on TypeName {
  field
  anotherField
}

query {
  ...MyFragment
}
```

## Variables

```graphql
query MyQuery($variable: String!) {
  fieldName(arg: $variable) {
    subField
  }
}
```

## Directives

```graphql
query MyQuery($includeSubField: Boolean!) {
  fieldName {
    subField @include(if: $includeSubField)
  }
}
```

## Aliases

```graphql
query {
  aliasName: fieldName {
    subField
  }
}
```

## Inline Fragments

```graphql
query {
  unionFieldName {
    ... on TypeName {
      field
    }
  }
}
```

## Introspection

```graphql
query {
  __schema {
    types {
      name
    }
  }
}
```
