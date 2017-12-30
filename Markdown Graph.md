# Markdown Graph

```flow
st=>start: Start
op=>operation: Choose
cd=>condition: yes/no
e=>end
st->op->cd
cd(yes)->e
cd(no)->op
```

```sequence
participant A
participant B
participant C
A->B: step 1
B->B: step 2
note right of A: note1
note left of B: note2
A-->C:step 3
B-->>C:step 4
C->A: over
```

```mermaid
gantt
dateFormat YYYY-MM-DD
title test
section study
	Quantum Mechanic: s1, 2018-01-17, 30day

section dating
	Girl1: d1,2018-01-20,1day
	Girl2: d2,after d1,1day

section photograph
	photo1: 2018-01-18, 2018-02-05
	photo2: 2018-02-05, 3day
```

