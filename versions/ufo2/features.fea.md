---
layout: default
title: features.fea
---

{: .fileformat}
| **File Format** | Plain Text |

This file contains the [Adobe Font Development Kit for OpenType] feature definitions. This file is optional. If it is not defined in the UFO, there is no feature data.

It is important to note that the features file may contain data that is a duplicate of or data that is in conflict with the data in [kerning.plist], [groups.plist] and [fontinfo.plist]. Synchronization between the files is not a requirement of this specification. Synchronization is up to the user and application developers.

## Specification

The file should be a plain text file and it should be in [AFDKO FEA syntax]. No assumption should be made about the validity of the syntax.

Any `include()` statements must be relative to the UFO path, _not_ to the `features.fea` file itself.

### Example

```fea
@myClass = [a b c];

feature liga {
  sub f i by fi;
  sub f l by fl;
} liga;
```


  [Adobe Font Development Kit for OpenType]: https://github.com/adobe-type-tools/afdko/
  [AFDKO FEA syntax]: https://adobe-type-tools.github.io/afdko/OpenTypeFeatureFileSpecification.html
  [kerning.plist]: ../kerning.html
  [groups.plist]: ../groups.html
  [fontinfo.plist]: ../fontinfo.html
