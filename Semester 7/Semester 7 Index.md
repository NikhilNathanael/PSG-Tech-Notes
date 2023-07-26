---
filetype : Index
tags : Semester7 SemesterIndex Index
---


# Subjects

```dataviewjs
let result = [];
for (x of dv.current().file.outlinks) {
  let notes = [];
  for (z of dv.page(x).file.outlinks) {
    if (dv.page(z).file.frontmatter.Filetype == "Notes") notes.push(z);
  }
  result.push([dv.fileLink(x.path,false, dv.page(x).file.frontmatter.Subject),notes]);
}
dv.table (["Subject", "Notes"],result);
```

%%
[[Supply Chain Management/Supply Chain Management Index|Supply Chain Management Index]]
[[Finite Element Analysis/Finite Element Analysis Index|Finite Element Analysis]]
[[Intellectual Property Rights/Intellectual Property Rights Index|Intellectual Property Rights]]
[[Refrigeration and Air Conditioning/Refrigeration and Air Conditioning Index|Refrigeration and Air Conditioning]]
[[Project Work/Project Work Index|Project Work Presentation]]
[[Internet of Things/Internet of Things Index|Internet of Things]]
[[Geometric Modelling/Geometric Modelling Index|Geometric Modelling]]
%% 
