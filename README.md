# ISBN Validation
![](https://img.shields.io/badge/Status-Inactive-critical.svg)

This is what I've been using to validate ISBNs before saving to a data-source in the [Open School Library](https://github.com/Programazing/OpenSchoolLibrary) project.

## Limitations

Currently there are a few imposed limitations on these methods.

* ISBNs must be passed as strings.
* Though they only accept strings the contents of those strings can only be numbers or they will return **false**.
* ISBN 13s can only start with 978.
  * I'm aware that 979 exists but haven't updated the code just yet.
 
## Usage
 
Make a reference to the DLL in your project.

Define a using statement

```csharp
using IsbnValidation;
```

Create a boolean to use.

```csharp
var isbnIsValid = Validate.ISBN10(isbnStringToValidate);
```
