# graphql-supergraph

```
rover subgraph publish supergraph-hp6gbp@current   \
    --schema graphql-order/src/main/resources/schema/schema.graphqls   \
    --name order   \
    --routing-url http://localhost:8081/graphql
```
```
rover subgraph publish supergraph-hp6gbp@current   \
    --schema graphql-customer/src/main/resources/schema/schema.graphqls   \
    --name customer   \
    --routing-url http://localhost:8082/graphql
```
```
APOLLO_KEY=<> APOLLO_GRAPH_REF=<>   ./router --config router-config.yaml
```
```
curl -sSL https://router.apollo.dev/download/nix/v1.46.0 | sh
```