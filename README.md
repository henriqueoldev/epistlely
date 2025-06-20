# Epistlely 📚

Epistlely is an open-source project built with **Astro.js**, designed for authors to publish their works statically using **Markdown**. With a responsive design and easy customization, it provides a simple and efficient way for writers to share their stories. 

## Features
- **Static Publishing**: Publish your writings using Markdown.
- **Responsive Design**: Works on most devices
- **Easy Customization**: Simple config files.

## Getting Started 🚀
### 1. Clone the Repository
Open your terminal and run the following command to clone the project:

```bash
git clone https://github.com/henriqueoldev/epistlely.git
```

### 2. Configure Author Information
Edit the author configuration in `/src/config/author.json`:

```json
{
  "name": "Your name",
  "description": "Your description",
  "profilepic": "/yourprofilepicture.exts"
}
```

### 4. Add Your Book .md Files
Place your book files in **/src/books/yourbook/**. They will be loaded in alphabetical order, so if you are numbering the files, use the following format:  
- For fewer than 10 files, name them 01.md to 09.md  
- For fewer than 100 files, name them 001.md to 099.md  
- And so on...

### 5. Register Your Books
Register your books in `/src/config/books.json` as follows, so they can be loaded:

- "path" is the folder name that contains your .md files, it **must** be inside **/src/books**
- "cover" is the book cover image, it **must** be inside **/public/covers**
```json
[
  {
    "title": "Book name",
    "description": "Book description",
    "path": "foldername",
    "cover": "covername.exts"
  }
]
```

### 5. Run the Project
Navigate to the project directory and start the development server:

```bash
cd epistlely
npm install
npm run dev
```

## Contributing
If you have suggestions or improvements, feel free to open an issue or submit a pull request.

---

## License 📄
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
