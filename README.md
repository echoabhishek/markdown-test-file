# Sample README for Testing Markdown Rendering

This README is designed to test different ways of embedding images, code blocks, and other markdown features. Below are examples with various styles.

---

## 1. Relative Image Paths

### a. Single Dot (Current Directory)
![Current Directory Image](./assets/flocking-birds-270-512x384.jpg)

### b. Double Dot (Parent Directory)
![Parent Directory Image](./assets/../assets/green-mountains-929-512x384.jpg)

---

## 2. Protocol-Less Paths

### a. Assets without Protocol
![Protocol-Less Image](assets/walk-pier-77-512x384.jpg)

### b. With `@` Alias Path (e.g., some setups use `@/` as a shortcut for root)
![Alias Path Image](@/assets/window-droplets-171-512x384.jpg)

---

## 3. Absolute URL (Direct HTTP Link)

Here’s an example using a direct HTTP link to an image:

![Direct HTTP Image](https://fastly.picsum.photos/id/270/512/384.jpg?hmac=7QIE6MrLtoPkj-Qb16FJHDR6p3VJyqoS8h5zMuLd75A)

---

## 4. HTML `<img>` Tag

Sometimes images are embedded using HTML directly:

*Absolute Url*

<img src="./assets/indoor-plant-305-512x384.jpg" alt="HTML Tag Image" width="200"/>

*Actual Url*

<img src="https://fastly.picsum.photos/id/1008/512/384.jpg?hmac=AliEcjRkF8CHy5RBfblxvkq6xTYGH23fjNhXmnmnCVE" alt="HTML Tag Image" width="200"/>

---

## 5. Markdown with Code Blocks

### JavaScript Code Block

```javascript
// JavaScript example
const fetchData = async () => {
  try {
    const response = await fetch('https://api.example.com/data');
    const data = await response.json();
    console.log(data);
  } catch (error) {
    console.error('Error fetching data:', error);
  }
};
fetchData();
```

### Python Code Block

```python
# Python example
def fetch_data():
    try:
        response = requests.get('https://api.example.com/data')
        data = response.json()
        print(data)
    except Exception as e:
        print(f"Error fetching data: {e}")

fetch_data()
```

### Inline Code and Emoji

This is a sample inline code `const example = true;` with some emojis 🚀✨ for testing.

---

## 6. Nested Directories for Images

Testing images in nested directories:

![Nested Image](./nested/folder/image-in-nested-folder.png)

---

## 7. Blockquotes and Lists

> This is a blockquote. It’s used to highlight some important information.

### Ordered List
1. First item
2. Second item
3. Third item with **bold text** and *italic text*

### Unordered List
- Item one
- Item two
- Item three

---

## 8. Tables

| Feature            | Supported | Notes                                    |
|--------------------|-----------|------------------------------------------|
| Relative paths     | ✅         | Tests relative paths for image loading.  |
| Protocol-less paths| ✅         | Tests assets without `http/https`.       |
| Code blocks        | ✅         | Tests various programming languages.     |
| Emojis             | ✅         | 😊 😎 👍                                  |

---

## 9. Task List

- [x] Test markdown rendering
- [x] Test image loading in various formats
- [ ] Check code block formatting
- [ ] Ensure emoji support


### Explanation of Markdown Elements

- **Image Loading**: The file includes various ways of referencing images, such as relative paths (`./assets/current-dir-image.png`), protocol-less paths (`assets/no-protocol-image.png`), alias paths (`@/assets/alias-path-image.jpeg`), direct HTTP URLs, and even an HTML `<img>` tag.
- **Code Blocks**: There are fenced code blocks in JavaScript and Python, which help you check syntax highlighting and formatting.
- **Inline Code and Emoji**: Inline code with emojis lets you verify proper rendering of special characters.
- **Lists and Blockquotes**: Basic list and blockquote elements for markdown structure testing.
- **Tables and Task Lists**: Tables test how tabular data is handled, and task lists check if your markdown renderer supports this GitHub feature.

### Using This for Testing

Add appropriate assets (image files) with the same names as specified in this markdown file to your test repository. This will ensure that each link or reference type points to an actual file, helping you observe how your rendering function handles each case.

Let me know if you need further customization of this README!

