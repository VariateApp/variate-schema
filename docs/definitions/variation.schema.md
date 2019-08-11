# Variation Schema

```
https://variate.ca/definitions/variation.json
```

The variation object contains the variation ID, traffic allocation information and the list of components for this
variation.

| Abstract            | Extensible | Status | Identifiable | Custom Properties | Additional Properties | Defined In                                                 |
| ------------------- | ---------- | ------ | ------------ | ----------------- | --------------------- | ---------------------------------------------------------- |
| Can be instantiated | No         | Draft  | No           | Forbidden         | Permitted             | [definitions/variation.schema.json](variation.schema.json) |

## Schema Hierarchy

- Variation `https://variate.ca/definitions/variation.json`
  - [ID](id.schema.md) `https://variate.ca/definitions/id.json`
  - [Traffic](traffic.schema.md) `https://variate.ca/definitions/traffic.json`

# Variation Properties

| Property                                  | Type     | Required     | Nullable | Defined by                                 |
| ----------------------------------------- | -------- | ------------ | -------- | ------------------------------------------ |
| [components](#components)                 | `object` | **Required** | No       | Variation (this schema)                    |
| [id](#id)                                 | ID       | **Required** | No       | Variation (this schema)                    |
| [traffic_allocation](#traffic_allocation) | Traffic  | **Required** | No       | Variation (this schema)                    |
| `*`                                       | any      | Additional   | Yes      | this schema _allows_ additional properties |

## components

### Component list

`components`

- is **required**
- type: `object`
- defined in this schema

### components Type

`object` with following properties:

| Property | Type | Required |
| -------- | ---- | -------- |


## id

### Variation ID

`id`

- is **required**
- type: ID
- defined in this schema

### id Type

- [ID](id.schema.md) – `https://variate.ca/definitions/id.json`

## traffic_allocation

`traffic_allocation`

- is **required**
- type: Traffic
- defined in this schema

### traffic_allocation Type

- [Traffic](traffic.schema.md) – `https://variate.ca/definitions/traffic.json`