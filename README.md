# Digital Twin document

This repository contains version 1.0 of a Digital Twin (DT) document standard. The DT document describes the metadata and features of a single digital twin. The document is designed to be used along with a Data Link that connects the features of the digital twin behind a single access point.

The format of the document is YAML and ``descriptions-of-terms.md`` describes fields of the DT document. The description contains both mandatory and optional fields.

The examples folder contains an example document ``crane-public.yaml`` following the DT document standard. In addition, there are two examples of files that provide additional information for the digital twin with different privacy classifications. These files use the field descriptions from ``descriptions-of-terms.md``. However, only id and privacy fields are mandatory.

## An example of a DT document's content

```
version: "1.0"
privacy: "public"
id: "http://lampthing.fi/lamp-L98765"
name: "Lamp in the fridge"
description: "Lamp installed in the fridge used to light up the refrigerator."
createdMachine: "1583195640"
createdHuman: "2020-03-02_19-34-00"
manufacturer: "Philips"
features:
  - name: "Sensor reading"
    description: "Sensor reading allows managing sensors attached to the lamp."
    address: "https://lamptwin.fi/sensors/browse"
    requirement: "User account is needed."
    keywords:
      - "sensors"
      - "measurement"
      - "temperature"
      - "management"
```

### Main mandatory terms

| Term | Subterms | Description | Assignment | Type |
| ------------- | ------------- | ------------- | ------------- | ------------- |
| version  |  | The version of the digital twin document | mandatory | string |
| privacy  |  | The privacy of the digital twin | mandatory | string |
| id  |  | The digital twin id | mandatory | string |
| name  |  | Name of the digital twin | mandatory | string |
| description  |  | The description of the digital twin | mandatory | string |
| createdMachine  |  | The creation date of the digital twin document (machine-readable) | mandatory | string |
| createdHuman  |  | The creation date of the digital twin document (human-readable)| mandatory | string |
