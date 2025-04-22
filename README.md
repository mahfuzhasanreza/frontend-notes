# Frontend Notes

# Note 1

## html: hypertext markup language


### 🟥 tag:
- `p`, `small`, `h1-h6`
- `b`, `strong`
- `i`, `em`
- `div` **(container tag)**

**🟥 Semantic tag:**  
Meaningful or something important  
**strong**, **em** are semantic tags

**🟥 Inline (in a line):**  
`strong`, `em`, `i`, `small`, `span`, `a`

**🟥 Block:**  
`p`, `h1-h6`, `div`, `p`

---

### 🟥 list + button:

- **Normal:** `li` (bullet point)

#### 🔸 Unordered list: `ul` **(container tag)**
- `li` (bullet point)
- `type = disc, circle, square, none`

#### 🔸 Ordered list: `ol` **(container tag)**
- `li` (1, 2, 3, ...)

#### 🔸 Button:
- `button`

---

### 🟥 HTML link (hyperlink):

- **External:** link  
- **Internal:** `~.html`

**Tag:** `a` (anchor)  
**Attribute:** `href` (hypertext reference)  
```html
<a href=""></a>
```

- `download` = download **(attribute)**  
- `target="_blank"` **(attribute)**

---

### 🟥 Image

- **Void tag:** `img` **(self-closing tag)**
- `src`: source  
- `alt`: alternative text

---

### 🟥 Form

**Tag:** `form` **(container tag)**  
- `action`: where to send the data  

**Tag:** `input` **(void/self-closing tag)** – *inline*  
- `type` (attribute) = text, password, email, number, date, checkbox, radio, file  
- `value` (attribute) = default, submit  
- `placeholder` (attribute) = hint  

**Tag:** `select`  
- `option`, `value` (attribute)

---

### 🟥 Structure

- `html > head > body > footer`  
- VSCode shortcut: `!`  
- Favicon  


# CSS Notes

## css: Cascading Style Sheets

### Syntax:
```css
selector {
  property: value;
}
```

---

## Types of CSS:
- Inline
- Internal/Embedded
- External

---

## CSS Selectors:
- ID: `#`
- Class: `.`
- Element
- Attribute

---

## Relative Units:
- `px`: 1/96th of 1in

### Relative/Comparative Units:
- `vh`: 1% of the viewport height
- `vw`: 1% of the viewport width
- `em`: relative to font-size of element
- `rem`: relative to root element (`html`)
- `vmin`: 1% of smaller viewport dimension
- `vmax`: 1% of larger viewport dimension
- `%`: relative to parent

---

## More CSS Selectors:
- Universal: `*`
- Type/Tag: `p`, `h1`, etc.
- Class: `.classname`
- ID: `#idname`
- Attribute: `[attribute]` (e.g. `input[required]{}`)
- Child: `parent > child`
- Grouping: `p, h1 {}`

### Font Weight:
- `400` = normal
- `700` = bold
- `900` = bolder

### ID Rules:
- One element cannot have more than 1 ID
- One page cannot have duplicate IDs

---

## CSS Margin, Padding, Height:

### Margin:
- `margin: top right bottom left;` (Clockwise)
- `margin: top-bottom right-left;`
- `margin: top right-left bottom;`
- `margin: all sides;`

### Padding:
- Same as margin

### Height:
- `max-height`: can be decreased
- `min-height`: can be increased

---

## CSS Box Model:
Box size depends on:
1. content
2. border
3. padding
4. margin
5. width and height (additional)

---

## CSS Display, Visibility, Box Shadow:

### Hide:
- `display: none;` (removes space)
- `visibility: hidden;` (retains space)

### Box Shadow:
```css
box-shadow: x y color;
box-shadow: x y blur;
box-shadow: x y blur color;
box-shadow: x y blur spread color;
```

### Inline Elements:
- `span` does not support height/width/margin fully
- Use `display: block;` to enable full layout support
- Or `display: inline-block;`

### Block Elements:
- `div` supports height, width, margin

---

## CSS Image:

```css
background-image: url('image.jpg');
background-size: cover; /* Fit and fill */
background-size: contain; /* Fit while keeping aspect ratio */
background-repeat: no-repeat;
background-repeat: repeat-x;
background-repeat: repeat-y;
background-position: center;
background-position: top;
background-position: left top;
```

---

## CSS Color:

- **Color Name**: `red`, `blue`, `green`, etc.
- **Hex**: `#RRGGBB` (e.g., `#FF5733`)
- **RGB**: `rgb(255, 87, 51)`
- **RGBA**: `rgba(255, 87, 51, 0.5)`