# Output Schemas

Output schemas specify how backends generate the output of a QIR program based on calls to [output recording functions](../profiles/Base_Profile.md#output-recording).

Each backend can decide which output schema to use depending on the characteristics of their system.

There are two output schemas:
- **[Ordered](./Ordered.md)**: for backends that synchronously emit output records and do not support strings as arguments to functions.
- **[Labeled](./Labeled.md)**: for backends that asynchronously emit output records and support strings as arguments to functions.

Grammars that define the structure and valid values for these schemas are available [here](./Grammars.md).

Additonal information and examples for implementators can be found [here](./Notes.md).