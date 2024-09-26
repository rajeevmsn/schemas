# schemas

JSON schemas for Connect

----------------
## Pull request to be approval checklist
  

- [ ] **Use Enums for Strings:** Ensure that all string-type properties are defined as enumerations (enums) wherever applicable to promote consistency and maintainability.

- [ ] **No Collection of Personal Identifiable Information (PII):** Verify that no personal identification information (PII) such as name, identification number, online identifier, sex, date of birth, address, location data, etc., is collected. For details, refer to the [GDPR Guidelines on Personal Data](https://gdpr-info.eu/issues/personal-data/).

- [ ] **Complete Property Definitions:** Provide clear and complete definitions and descriptions for all properties to ensure proper understanding and usage across the team.

- [ ] **Required Fields:** List all mandatory fields under the `"required"` keyword to avoid schema violations and make it clear what properties must always be included in valid objects.

- [ ] **Type Validation:** Ensure that each property has an explicitly defined type (`string`, `number`, `boolean`, `array`, `object`, etc.) and that arrays and objects have well-defined item structures.

- [ ] **Avoid Redundancy:** Ensure there are no duplicate or redundant fields. Consolidate where necessary and avoid conflicting properties.

- [ ] **Consistent Naming Convention:** Follow a consistent naming convention for all property names. E.g., `camelCase` for JavaScript-based projects or `snake_case` for Python-based projects.

- [ ] **References (**`$ref`**) for Reusable Components:** Use `$ref` to reference reusable schema components to avoid duplication and promote consistency across the schema.

- [ ] **Additional Properties:** Explicitly specify whether additional properties are allowed by setting `"additionalProperties": false` if only defined fields should be present in the object.