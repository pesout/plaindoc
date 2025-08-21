# Plaindoc Cheatsheet

- Plaindoc is a formatting style for plaintext documents (`.txt`) in places where markdown couldn't be displayed graphically

**Basic principles**

- Leave 1 blank line between blocks
- Keep ~80 characters per line

## Headings

```txt
DOCUMENT TITLE
==============
```

```txt
Chapter
-------
```

```txt
[Subsection]
```

## Paragraphs and emphasis

```txt
This is text in a paragraph. No special formatting required.
```

Some text can be `*IMPORTANT*`, contain `/light emphasis/` and also `=inlineCode()=`.

Paragraph can contain inline links: `(> https://example.com)`.

## Lists and quotes

**Bullets**

```txt
- Top level
- Also top level
	- Nested item
	- Other nested item
- Other top level
```

**Numbering**

```txt
1) First
2) Second
3) Third
```

**Checklist (tasks)**

```txt
[ ] Open
[x] Done
[-] Partial / In progress
```

**Tasks with priorities**

```txt
[L][ ] Low priority
[M][ ] Medium priority
[H][ ] High priority
[C][ ] Critical priority
```

## Callouts

**Compact style**

```txt
[NOTE] A usage tip
[INFO] Some interestring info
[WARN] Beware of side effects
[TODO] Finish something later
```

**Box style**

```txt
+-------------------------+
| INFO: This is important |
+-------------------------+
```

## Code blocks

```txt
~~ (JAVASCRIPT)
const log = (data) => {
	console.log(data);
	return data;
}
~~
```

## Tables

**Full table**

```txt
+----------+--------+-------+
| Column A | B (ms) | C (%) |
+----------+--------+-------+
| alpha    |  123   | 98.2  |
| beta     |   87   | 76.0  |
+----------+--------+-------+
```

**Minimal table**

```txt
 Column A | B (ms) | C (%)
----------+--------+-------
 alpha    | 123    | 98.2
 beta     |  87    | 76.0
```

## Definition lists

```txt
FIRST TERM:
  Short explanation of the term.

SECOND TERM:
  Other short explanation of the term.
```

## File metadata (header)

```txt
@title: Document title
@date:  2025-01-01 00:00
@proj:  My project
@tags:  short, relevant, tags
```

## References

**In a paragraph**

```txt
This paragraph [1] contains references [2].
```

**At the end of the file**

```txt
REFERENCES
	[1] First reference: https://example.com/api/docs
	[2] Second reference: https://about.example.com
```

