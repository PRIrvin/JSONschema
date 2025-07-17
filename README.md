# JSONschema

**JSONschema** is a LabVIEW library designed to generate [JSON Schema](https://json-schema.org/) specifications from LabVIEW datatypes. It is built on top of [JSONtext](https://lavag.org/files/file/294-jsontext/), extending it with additional methods for schema-specific keywords such as `minimum`, `maximum`, and more.

The library was originally developed for use by the [Instrument Framework](https://github.com/levylabpitt/Instrument-Framework), but is useful for any LabVIEW developer needing to serialize or validate LabVIEW data structures as JSON according to a formal schema.

## Features

- Generate JSON Schemas directly from LabVIEW typedefs and variants.
- Annotate schemas with additional keywords (e.g., value constraints).
- Convert between JSON Schema and tabular representations.
- Pretty-print JSON Schemas for documentation or review.

## Getting Started

- Developed and packaged in **LabVIEW 2019**.
- Install via VI Package Manager. Detailed instructions: [levylabpitt.github.io](https://levylabpitt.github.io/)

## API Methods

The main API VIs are located in `JSON-Schema/API/`. Core API methods include:

- **Create JSON Schema (Interactive).vi**  
  Launches an interactive dialog to create a JSON Schema from a LabVIEW datatype.

  ![image](https://github.com/user-attachments/assets/f38563a9-28d9-40d6-aa7c-93240cf3ca31)

- **Create JSON Schema.vi**  
  Programmatically generate a JSON Schema from a LabVIEW datatype.

  <img width="344" height="191" alt="image" src="https://github.com/user-attachments/assets/d2cbb44b-3f76-4aec-9e53-70c897e961b0" />

- **Initialize JSON Schema.vi**  
  Set up a new JSON Schema document.

  <img width="369" height="148" alt="image" src="https://github.com/user-attachments/assets/3064238e-0e06-48be-a27b-5c37acdc6419" />

- **Choose JSON Schema Dialect.vi**  
  Select the JSON Schema dialect/version to use.

  <img width="392" height="234" alt="image" src="https://github.com/user-attachments/assets/4fa4cf12-5bd1-4c48-8619-efba1a5168a0" />

- **Read Typedef Description.vi / Read Typedef Description (variant).vi / Read Typedef Description (path).vi**  
  Read and interpret the description of a typedef from a reference, variant, or file path.
  
  <img width="346" height="109" alt="image" src="https://github.com/user-attachments/assets/51bcc2b4-311d-4319-aa60-d7005528acae" />
  <img width="340" height="104" alt="image" src="https://github.com/user-attachments/assets/04d6de29-a505-4fa2-9051-b2128467f29d" />

- **Write Typedef Description.vi / Write Typedef Description (variant).vi / Write Typedef Description (path).vi**  
  Write or update the description of a typedef in various forms.

  <img width="360" height="108" alt="image" src="https://github.com/user-attachments/assets/52202aca-2fd7-4246-910b-5276c0a34d15" />
  <img width="364" height="110" alt="image" src="https://github.com/user-attachments/assets/f3cd51a1-ce5c-40ab-8c61-e4f3a32fc19e" />

- **Add Object to JSON Schema.vi**  
  Insert a new object definition into the schema.

  <img width="368" height="110" alt="image" src="https://github.com/user-attachments/assets/1fdb95cd-f1c2-4e6c-9aa2-24f52f778995" />

- **JSON Schema Pretty Print.vi**  
  Output the JSON Schema in a human-readable format.

  <img width="342" height="90" alt="image" src="https://github.com/user-attachments/assets/878de7f7-7ee8-4194-8844-d6f03b7c1506" />

- **JSON Schema to Table.vi / Table to JSON Schema.vi**  
  Convert between JSON Schema and a tabular representation for easier manipulation or review.
  
  <img width="371" height="105" alt="image" src="https://github.com/user-attachments/assets/e4a0db23-a4cb-4cc7-8dba-f0eb648a8a72" />
  <img width="366" height="103" alt="image" src="https://github.com/user-attachments/assets/ab939ef1-c54f-48e3-8417-58078f46ac62" />

## Examples
- see **Create JSON Schema (Interactive).vi**  

## Dependencies

- [JSONtext](https://lavag.org/files/file/294-jsontext/)

## Contributing

Feedback and contributions are welcome!  
Contact [Patrick Irvin](https://github.com/ciozi137) for more information.

## License

[BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)
